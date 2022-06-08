pipeline {
	//agent any
	//agent { docker { image 'maven' }} 
	agent { docker { image 'node' }}
	stages {
		stage('Build') {
			steps {
			    //sh "mvn --version"
				sh "node --version"
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo " im awesome " }
		success {
			echo " iam sucessful" }
		failure {
			echo "failed" }
	}
}
