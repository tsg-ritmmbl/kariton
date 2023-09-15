pipeline {
  agent any
  stages {
    stage('Install Nextflow') {
      agent any
      steps {
        sh 'curl -s https://get.nextflow.io | bash'
      }
    }

  }
}