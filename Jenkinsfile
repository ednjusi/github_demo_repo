//  Scripted Pipleine
// node {
// 		echo "Build"
// 		echo "Test"
// 		echo "Intergration Test"
// 	}

// Declarative pipeline
 pipeline {
	    // agent any
		agent {docker {image 'node:13.8'}}
		stages {
			stage('Build') {
				steps {
                    // sh 'mvn --version'
					sh 'node --version'
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
		
		
		} 
		
		post {
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