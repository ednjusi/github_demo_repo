//  Scripted Pipleine
// node {
// 		echo "Build"
// 		echo "Test"
// 		echo "Intergration Test"
// 	}

// Declarative pipeline
 pipeline {
	    agent any
		stages {
			stage('Build') {
				steps {
			echo "Build"	
				}
			}
			stage('Test') {
				steps {
			echo "Test"
				}
			}
			stage('Intergration Test') {
				steps {
			echo "Intergration Test"
				}
			}
		
		
		} post {
			always {
				echo 'Im awesome. I run always'
			}
			success {
				echo 'I run when you are successful'
			}
			failure {
				echo 'I run when you fail'
			}
		}
		
	}