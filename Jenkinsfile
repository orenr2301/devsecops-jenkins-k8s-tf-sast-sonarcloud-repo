pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=orenr2301 -Dsonar.organization=orenr2301 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=bb31b725e0926a4b0b0104af44445a23e4218dc6'
			}
        } 
  }
}
