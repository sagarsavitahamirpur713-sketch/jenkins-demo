pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/username/repository.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }
    }
}


pipeline {
agent any
triggers { pollSCM('H/2 * * * *') }
stages {
stage('Build') { steps { sh 'sh app.sh' } }
stage('Test')  { steps { sh 'sh test.sh' } }
stage('Deploy') { steps { echo 'Deploying...' } }
}
}
