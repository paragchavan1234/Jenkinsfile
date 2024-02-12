pipeline {
    agent {
        docker {
            image 'your-docker-image:tag'
            args '-v /host/path:/container/path'
        }
    }
    stages {
        stage('Build') {
            steps {
                // Your build steps here
            }
        }
        // Add more stages as needed
    }
}
