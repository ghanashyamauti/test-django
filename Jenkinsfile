pipeline {
    agent any

    environment {
        NAME = 'Ghanashyam'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Compiling code...'
                echo "Compiled by ${NAME}"
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to server...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
