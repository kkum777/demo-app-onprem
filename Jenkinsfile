def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any

  stages {
	
	stage('Publish to Exchange') {
         steps {
		   	bat  'mvn -s C:\Users\gvkk1\.m2\settings.xml -X  clean deploy'
		 }
		 }
	stage ('Deploy to On-prem') {
            steps {
			bat 'mvn -s C:\Users\gvkk1\.m2\settings.xml -X  clean deploy -DmuleDeploy'
      }
    }
   }
   }
