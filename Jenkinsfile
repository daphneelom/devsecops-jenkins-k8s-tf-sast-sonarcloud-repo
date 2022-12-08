pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonacloud -Dsonar.organization=sonacloud -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=a43e314ad40f9159d43429ac2b4408d451d48e06
			}
        } 
  }
}
