# mmgenome_notes
Notes about mmgenome workflow (http://madsalbertsen.github.io/mmgenome/)

## Generates data 
From Script: https://github.com/MadsAlbertsen/mmgenome/blob/master/workflows/data.generation.2.1.0.sh
- Use the latest version of Prodigal (https://github.com/hyattpd/prodigal/releases/)
- Use MEGAN v4

From PhylopythiaS+:
- This software is not available. Alternative way: https://github.com/JeremieMG/Alternative-PPSP-output 

## Loading data
Tutorial: http://madsalbertsen.github.io/mmgenome/Load_data.html
- Add an additional option to load the "alternative ppsp output" (quote = ""):
```
pps <- read.table("data/pps.txt", sep = "\t", quote = "", header = F, col.names = c("scaffold","pps_root", "pps_kingdom", "pps_phylum", "pps_class", "pps_order", "pps_family", "pps_genus", "pps_species"))[,c(1,4,5,6,7,8)]
```

## Using mmgenome on R
Tutorial: http://madsalbertsen.github.io/mmgenome/Genome_extraction.html
- Do not use mmgenome library on R Studio. Takes R on terminal.
