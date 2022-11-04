pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }
    environment {
    	TEST_VARIABLE = 'TEST'
        BUILD= "TEST_BUILD"
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
    post{
    	always{
    		 mail to: 'jsiow002.dev@gmail.com',
             subject: "First pipeline ",
             body: "${TEST_BUILD}"
    	}
    }
}
