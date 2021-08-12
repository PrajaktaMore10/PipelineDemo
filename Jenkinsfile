pipeline {
	 agent any
		stage('Compile Stage'){
			steps{
				withMaven(maven: 'maven_3_5_0') {
					sh 'mvn clean compile'
					}
				}	
			}
			
		stage('Testing Stage'){
				steps{
				withMaven(maven: 'maven_3_5_0') {
					sh 'mvn Test'
					}
				}	
			}
		stage('Deployment Stage'){
				steps{
				withMaven(maven: 'maven_3_5_0') {
					sh 'mvn Deploy'
					}
				}	
			}
        }
