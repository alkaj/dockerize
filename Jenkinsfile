pipeline {
	agent {
		docker {
			image "docker:dind"
			pullPolicy "Never"
		}
	} 
	stages {
		stage('Build') {
			steps {
				echo 'Building the image container'
				sh "docker build -t alkaj/dockerizer:${BUILD_NUMBER}"
			}
		}
		stage('Test') {
			steps {
				echo 'Checking the image container'
				sh "docker run --rm alkaj/dockerizer:${BUILD_NUMBER}"
			}
		}
		stage('Deploy') {
			steps {
				echo 'Pushing the image container to docker hub'
			}
		}
	}
}