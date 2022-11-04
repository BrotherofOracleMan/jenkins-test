/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }
    stages {
        stage('Test') {
            steps {
                sh 'This is Test step'
            }
        }
    }
    post {
    	always{
    		echo 'This will always be run'
    	}
    	success{
    		echo 'This will only run if successful'
    	}
    }
}
