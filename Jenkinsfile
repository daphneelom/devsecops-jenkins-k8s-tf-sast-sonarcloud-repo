pipeline {
  agent any
  tools { 
        maven 'Maven 3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=christiane -Dsonar.organization=christiane -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=29ba547eaa61d390187a3af28023f6772bf95211'
			}
        } 
  }
}
