def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any

  stages {
	stage('Publish to Exchange') {
         steps {
		   bat 'mvn -s C:/Users/gvkk1/.m2/settings.xml clean deploy'
		 }
		 }
	stage ('Deploy to OnPrem') {
            steps {
			bat 'mvn -s C:/Users/gvkk1/.m2/settings.xml clean deploy -DmuleDeploy'
      }
    }
   }
   
   
}