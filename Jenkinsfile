pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=anbuggywebapp -Dsonar.organization=anbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6ee997986402d8925fa3e34e19027ad64c82f589'
			}
        } 
  }
}
