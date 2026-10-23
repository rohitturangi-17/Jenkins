
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Starting Jenkins pipeline'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
                sh 'mkdir -p build'
                sh 'echo "Hello from Jenkins" > build/output.txt'
            }
        }

        stage('Test') {
            steps {
                sh 'cat build/output.txt'
                echo 'Test completed successfully'
            }
        }
    }
}
