pipeline {
  agent any
  stages {
    stage('Clone Repository') {
      agent any
      steps {
        sh 'git clone https://github.com/tsg-ritmmbl/kariton.git'
      }
    }

  }
  environment {
    nextflow = ''
  }
}