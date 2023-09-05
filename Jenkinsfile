pipeline {
	agent any
	tools {
		nextflow
	}
	parameter {
		choice
	}
	stages {
		stage("build") {
			steps {
				echo 'building the application...'
			}
		}
		stage("test") {
			when {
				expression {
				
				}
			}
			steps {
				echo 'testing the application...'
			}
		}
		stage("deploy") {
			steps {
				echo 'deploying the application...'
			}
		}
	}
}
