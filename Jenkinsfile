pipeline {
  agent any
  stages {
    stage('Run Pipeline') {
      steps {
        sh '''#!/bin/bash

# Set the path to your Nextflow pipeline repository
PIPELINE_REPO="https://github.com/your-username/your-pipeline-repo.git"

# Set any required input parameters for your Nextflow pipeline
BAMMIX_FILE="/mnt/c/Users/MBL-IT/Desktop/kariton_data/flagged_barcodes_positions_proportions.csv"
REF_FILE="/mnt/c/Users/MBL-IT/Desktop/kariton_data/Barcode_Batch08.csv"
BAM_DIR="/mnt/c/Users/MBL-IT/Desktop/kariton_data/articNcovNanopore_sequenceAnalysisNanopolish_articMinIONNanopolish/"
FASTA_DIR="/mnt/c/Users/MBL-IT/Desktop/kariton_data/articNcovNanopore_prepRedcap_renameFasta/"
OUT_DIR="/mnt/c/Users/MBL-IT/Desktop/kariton_data/result"

# Navigate to the directory where you want to run the pipeline
cd /mnt/c/Users/MBL-IT/Desktop/kariton_data/test_run

# Clone the pipeline repository (if not already cloned)
git clone $PIPELINE_REPO

# Navigate to the cloned repository directory
cd your-pipeline-repo

# Run the Nextflow pipeline with the specified parameters
nextflow run kariton \\
    --bammix $BAMMIX_FILE \\
    --ref $REF_FILE \\
    --bam_dir $BAM_DIR \\
    --fasta_dir $FASTA_DIR \\
    --out_dir $OUT_DIR
'''
      }
    }

  }
}