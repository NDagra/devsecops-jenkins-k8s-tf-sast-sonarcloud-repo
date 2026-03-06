pipeline {
  agent any
  tools { 
        maven 'Maven_3.8.4'
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=batcave2026 -Dsonar.organization=Batcave -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=81a2c7052f4b8fb55dc9dcff86581a216b4b31e1'
			}
        } 
  }
}
