pipeline {
	agent {
		docker {
			image "node:alpine"
		}
	} 
	stages {
		stage('Build') {
			steps {
				echo 'Building the image container'
				sh 'node -v'
			}
		}
		stage('Test') {
			steps {
				echo 'Checking the image container'
				sh 'npm install'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Pushing the image container to docker hub'
			}
		}
	}
}