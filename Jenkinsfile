pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test commands here, e.g., npm test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'npm start &'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing...'
                // Add your release commands here
            }
        }
        stage('Monitoring and Alerting') {
            steps {
                echo 'Monitoring...'
                // Add your monitoring setup commands here
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

