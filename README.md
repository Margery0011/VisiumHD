# VisiumHD

`Spaceranger` updated to Version3.0.1, download from [10x website](https://www.10xgenomics.com/support/software/space-ranger/downloads/space-ranger-installation)
Installed on linux server

## Run example
```
/mnt/scratch1/spaceranger/spaceranger-3.0.1/spaceranger/spaceranger-3.0.1/bin/spaceranger count --id=H128FR87Z-D1-F \
--transcriptome=/reference/transcript \
--fastqs=/path/to/fastq/ \
--probe-set=/path/to/probe-set \
--cytaimage="path/to/tif" \
--image="/path/to/H&E/" \ # optional, suggest do not use for better alignment
--slide=H1-28FR87Z \ # optional
--area=D1 \# optional
--create-bam=false
```
*Notes*:
Space Ranger v3.0 and later requires the --create-bam argument to be set to true or false. Here, we set it to false to save disk space and computation time. BAM files can be useful for long term data archiving, troubleshooting (especially mapping), and other reasons.
