def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any

  stages {
	stage('Build') {
         steps {
		   bat 'mvn  clean package -DskipTests'
		 }
		 }
	
	stage ('Deploy to On-prem') {
            steps {
			bat 'mvn clean deploy -DmuleDeploy'
      }
    }
   }
   }