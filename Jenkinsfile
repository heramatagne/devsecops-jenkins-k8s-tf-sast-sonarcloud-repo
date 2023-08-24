pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sc-project2 -Dsonar.organization=sc-project2 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c1ebca9e8f7a520a11a2122c6abe24de763ab069'
			}
        } 
  }
}
