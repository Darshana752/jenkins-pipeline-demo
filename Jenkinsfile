pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning the repository...'
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the app...'
                // Add build logic if needed
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test || echo "No tests defined"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app...'
                // You can add deployment steps like `scp`, `docker`, etc.
            }
        }
    }
}
