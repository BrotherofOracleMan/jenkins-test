pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }
    environment {
    	TEST_VARIABLE = 'TEST'
    }
    stages {
        stage('build') {
            steps {
            	echo "Test variable output is : ${TEST_VARIABLE}"
                sh 'python --version'
            }
        }
    }
    post{
    	always{
    		echo 'This will always be run'
    	}
    
    }
}
