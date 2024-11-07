pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gpssecurityapp -Dsonar.organization=Gpssecurityapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a306381ca6b8642fdeba68812349eb220fa70d04'
			}
        } 
  }
}
