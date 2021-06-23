
//Declarative
pipeline {
	//agent any
	agent { docker { image 'node:13.8'}}
	stages {
		stage('Build') {
			steps {
			sh 'node --version'
			echo "Build"
			}
		}
		
		stage('Test') {
			steps {
			echo "Test"
			}
		}
		
		stage('Integration test') {
			steps {
			echo "Integration test"
			}
		}
	}

	post {
		always {
			echo 'Im awesome'
		}
		success { 
			echo 'successful'
		}
		failure { 
			echo 'failed'
		}
	}
}