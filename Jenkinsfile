def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any

  stages {
	stage('Build') {
         steps {
		   bat 'mvn  clean deploy'
		 }
		 }
	
	stage ('Deploy to On-prem') {
            steps {
			bat 'mvn clean deploy -DmuleDeploy'
      }
    }
   }
   }