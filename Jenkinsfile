// SCRIPTED SYNTAX
// node {
// 	echo "Build"
// 	echo "Test"
// 	echo "Integration Test"
// }
// DECLARATIVE SYNTAX
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo "Build"
			}
		}
		stage('Test') {
			echo "Test"
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
}