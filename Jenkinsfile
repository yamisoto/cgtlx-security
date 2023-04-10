pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_1'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cgtlxprojects -Dsonar.organization=cgtlxprojects -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=bc1qs8x6caxpkns9szm37d8csd6ej4nr67qx3hk732'
			}
        } 
  }
}
