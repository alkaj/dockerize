pipeline {
	agent any 
	stages {
		stage('Build') {
			steps {
				echo 'Building the image container'
			}
		}
		stage('Test') {
			steps {
				echo 'Checking the image container'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Pushing the image container to docker hub'
			}
		}
	}
}