pipeline{
	
			agent any
			
			stages{
					stage ('scm checkout')
					
					{
						steps{
						
						branch: 'master,'git:"https://github.com/sidevops/maven-project.git"
						
						}
					
					
					}
			
			stage ('validate code')
			
			{
			
				steps{
				withMaven(jdk: 'localjdk-1.8', maven: 'localmaven') {
					sh 'mvn validate' 
					}
				
				}
			}
			
			}
	
	
}
	
	
