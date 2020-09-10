# Novel meta-analysis pipeline reveals dysregulated gene interactions and pathways in asthma



# Scripts/Deliverables 

pipeline.R: Main pipeline

pipeline.html: Static example of the R session (reproduction of the pipeline.R results)

# Dependencies

The following dependencies will be needed to run the main script. Please run this code in your Rsession to load in the appropriate dependencies.

```install.packages(c("MetaIntegrator", "igraph", "reshape2", "ggplot2", "BiocManager"))```


```BiocManager::install(c("WGCNA", "flashClust", "org.Hs.eg.db", "multtest"))```

# How to Run

```
git clone https://github.com/bg459/asthma_meta_analysis.git
cd asthma_meta_analysis
unzip data.zip
mv pipeline.R data
cd data
Rscript pipeline.R
```
Alternatively, pipeline.R can be run line-by-line or based on certain sections.
# Raw Data Files

A zip file (data.zip) is included with all the raw data, with the exact names as referenced in the program. To use these datasources, please unzip the file and move the folder's contents into the working directory. 

The following data files are included in data.zip: 

Microarray data: healthy.csv, disease.csv (Singhania et al.); healthy63.csv, disease63.csv (Wenzel et al.); healthy65.csv, disease65.csv (Yang et al.).

Transcription factor data: tfdb.csv (curated from TFDB database)

Differentially Expressed Genes: degenes1.csv (results from MetaIntegrator)

More specific methodologies of these data files are outlined in Methods section of manuscript.

# Other

All analysis was performed with R version 3.6.0 on a 64-bit MacBook Pro with 8 GB RAM. 
