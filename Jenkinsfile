pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggyapp -Dsonar.organization=asgbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f92274ea4db22be7e067f0c424258d59ffb3ca64'
			}
        } 
  }
}
