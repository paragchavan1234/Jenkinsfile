pipeline {
    agent {
        docker {
            image 'your-docker-image:tag'
            args '-v /host/path:/container/path'
        }
    }
    environment {
        // Add environment variables as needed
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Your build steps here
                sh 'echo "Building"'
            }
        }
        stage('Test') {
            steps {
                // Your test steps here
                sh 'echo "Testing"'
            }
        }
        stage('Deploy') {
            steps {
                // Your deployment steps here
                sh 'echo "Deploying"'
            }
        }
        // Add more stages as needed
    }
    post {
        success {
            // Actions to perform on success
            echo 'Build and tests passed!'
        }
        failure {
            // Actions to perform on failure
            echo 'Build or tests failed!'
        }
        always {
            // Actions to perform always, regardless of success or failure
            echo 'Cleaning up'
        }
    }
}
