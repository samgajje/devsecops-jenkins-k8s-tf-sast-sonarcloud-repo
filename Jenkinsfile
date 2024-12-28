pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=rjgbuggywebapp -Dsonar.organization=rjgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d109ab35e3bb1c688b3155a35dfb534735585f0e'
			}
        } 
  }
}
