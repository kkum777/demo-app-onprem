def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any

  stages {
	
	stage('Publish to Exchange') {
         steps {
		   	bat  'mvn clean deploy'
		 }
		 }
	stage ('Deploy to On-prem') {
            steps {
			bat 'mvn clean deploy -DmuleDeploy'
      }
    }
   }
   }
