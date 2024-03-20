pipeline {
  agent any
  tools { 
        maven 'maven_3.9.6'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Devsecops0107 -Dsonar.organization=Devsecops0107 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b6b27cb373fa90166313fad7c11ed35c171235a5'
			}
        } 
  }
}
