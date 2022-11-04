pipeline {
    agent any
    environment {
    	TEST_VARIABLE = 'TEST'
    }
    stages {
        stage('build') {
            steps {
                sh './gradlew check'
            }
        }
    }
    post{
    	always{
    		junit 'build/reports/**/*.xml'
    	}
    
    }
}
