pipeline {
	agent any
	//agent { docker { image 'maven' }} 
	//agent { docker { image 'node'}}
	stages {
		stage('Build') {
			steps {
			    //sh "mvn --version"
				//sh "node --version"
				echo "Build"
				echo "BUILD_NUMBER  $env.BUILD_NUMBER"
				echo "BUILD_ID  $env.BUILD_ID"
				echo "JOB_NAME  $env.JOB_NAME"
				echo "BUILD_TAG $env.BUILD_TAG"
				echo "BUILD_URL $env.BUILD_URL"
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
