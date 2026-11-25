pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'uname -a'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'test 1 -eq 1'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'echo Deployment successful!'
            }
        }
    }
}
