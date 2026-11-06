pipeline {
    agent any

    environment {
        IMAGE_NAME = 'shopease'
    }

    stages {
        stage('Checkout') {
            steps { checkout scm }
        }
        stage('Build Docker image') {
            steps {
                bat 'docker build -t %IMAGE_NAME%:%BUILD_NUMBER% .'
            }
        }
    }

    post {
        success { echo 'ShopEase Docker image built successfully.' }
        failure { echo 'Build failed. Check the stage logs.' }
    }
}
