pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=learning123 -Dsonar.organization=learning1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fc354fcd3fd7e6f4046176443d113f2de5461625'
			}
        } 
  }
}
