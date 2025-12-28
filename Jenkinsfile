pipeline {
    agent any

    environment {
        IMAGE_NAME = "stkramanuja/ram"
    }

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t %IMAGE_NAME%:latest .'
            }
        }
    }
}
