pipeline {
    agent any

    environment {
        IMAGE_NAME = "stkramanuja/ram"
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/stkramanuja-commits/Ram.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t %IMAGE_NAME%:latest .'
            }
        }
    }
}
