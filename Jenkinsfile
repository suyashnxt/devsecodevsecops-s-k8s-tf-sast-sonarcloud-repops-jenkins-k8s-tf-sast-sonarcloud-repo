pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapplication -Dsonar.organization=buggywebapplication -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=308a16b75f743c1537f9589567fb0fe214ad073'
			}
        } 
  }
}
