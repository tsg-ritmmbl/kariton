pipeline {
  agent any
  stages {
    stage('Clone Repository') {
      agent any
      steps {
        sh '''which nohup
sudo apt-get install nohup
echo $PATH
git clone https://github.com/tsg-ritmmbl/kariton.git'''
      }
    }

  }
  environment {
    nextflow = ''
  }
}