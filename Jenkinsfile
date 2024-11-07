pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gpsecurityapp -Dsonar.organization=GPsecurityapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=dfa1022d605958d8c0d67218177bd9fdcaed25cb'
			}
        } 
  }
}
