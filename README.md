# Novel meta-analysis pipeline reveals dysregulated gene interactions and pathways in asthma

# Brandon Guo (1), Sandra Andorf (1,2,3), Kari C. Nadeau (1†), Abhinav Kaushik (1†)
(1) Sean N Parker Center for Allergy and Asthma Research at Stanford University, Stanford University, Stanford, CA 94305–5101, USA
(2) Department of Pediatrics, University of Cincinnati College of Medicine, Cincinnati, OH, USA
(3) Divisions of Biomedical Informatics and Allergy & Immunology, Cincinnati Children’s Hospital Medical Center, Cincinnati, OH, USA 
(†) Corresponding author


# Scripts/Deliverables 

pipeline.R: Main pipeline

pipeline.html: Markdown file of pipeline results (same code as pipeline.R)

# Dependencies

The following dependencies will be needed to run the main script. Please run this code to load in the appropriate dependencies.

```install.packages(c("MetaIntegrator", "igraph", "reshape2", "ggplot2", "BiocManager"))
BiocManager::install(c("WGCNA", "flashClust", "org.Hs.eg.db"))```

# Raw Data Files

A zip file (data.zip) is included with all the raw data, with the exact names as referenced in the program. To use these datasources, please unzip the file and move the folder's contents into the working directory. 

The following data files are included in data.zip: 

Microarray data: healthy.csv, disease.csv (Singhania et al.); healthy63.csv, disease63.csv (Wenzel et al.); healthy65.csv, disease65.csv (Yang et al.).

Transcription factor data: tfdb.csv (curated from TFDB database)

Differentially Expressed Genes: degenes1.csv (results from MetaIntegrator)

More specific methodologies of these data files are outlined in Methods section of manuscript.

# Other

All analysis was performed with R version 3.6.0 on a 64-bit MacBook Pro with 8 GB RAM. 
