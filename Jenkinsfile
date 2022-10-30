pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=babawebapp -Dsonar.organization=babawebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=509e66e5e26ea43c4030cad1368a714c9c840374'
			}
        } 
  }
}
