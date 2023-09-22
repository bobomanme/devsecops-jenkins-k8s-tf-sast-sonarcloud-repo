pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bobomanme -Dsonar.organization=bobomanme -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0278f795de67135cd13000166eb8c91e835b68d4'
			}
    }
  }
}
