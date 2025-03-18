pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    echo 'Checking out the repository...'
                    checkout scm
                }
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                bat 'echo Build step executed'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Tests executed'
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
