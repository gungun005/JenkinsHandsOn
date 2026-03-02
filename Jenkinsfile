pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                echo "Installing dependencies..."
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
                sh 'bash test.sh'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }
    }

    post {
        success {
            echo "Pipeline Succeeded"
        }
        failure {
            echo "Pipeline Failed"
        }
    }
}
