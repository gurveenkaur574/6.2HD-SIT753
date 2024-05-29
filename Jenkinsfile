pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'echo Build step executed' // Use bat for Windows
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'echo Test step executed' // Use bat for Windows
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'echo Deploy step executed' // Use bat for Windows
            }
        }
    }
    post {
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
