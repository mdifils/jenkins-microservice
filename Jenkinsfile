// SCRIPTED SYNTAX
// node {
// 	echo "Build"
// 	echo "Test"
// 	echo "Integration Test"
// }
// DECLARATIVE SYNTAX
pipeline {
	// agent any
	agent { docker { image 'maven:3.8.4' } }
	// environment {
	// 	dockerHome = tool 'myDocker'
	// 	mavenHome = tool 'myMaven'
	// 	PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	// }
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				// sh 'docker version'
				// echo "Build"
				// echo "PATH - $PATH"
				// echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				// echo "BUILD_ID - $env.BUILD_ID"
				// echo "BUILD_TAG - $env.BUILD_TAG"
				// echo "JOB_NAME - $env.JOB_NAME"
				// echo "BUILD_URL - $env.BUILD_URL"
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
			echo "I always run"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "I run when you fail"
		}
	}
}