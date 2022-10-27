pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=femibuggywebapp -Dsonar.organization=femibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6e41ea898520058e0fba80ebc273e0bb69378fc8'
			}
        } 
  }
}
