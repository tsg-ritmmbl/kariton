pipeline {
  agent any
  stages {
    stage('AntArtic:nextcladeDL') {
      steps {
        sh '''mkdir nextclade
nextclade dataset get --name "sars-cov-2" --output-dir "nextclade"'''
      }
    }

  }
  environment {
    nextflow = ''
  }
}