pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }
    environment {
    	TEST_VARIABLE = 'TEST'
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
