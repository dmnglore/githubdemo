pipeline{
	agent any
	tools{
			maven 'Maven_3.9.6'
		}
	
	stages{
		stage('Build Maven'){
			steps{
			    checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/dmnglore/jenkins-docker-sample']])
			    bat 'mvn clean install'
			}
		}
		
			stage('build') {
            steps {
                echo  'build done'
            	}
        	}
         }
    }	
