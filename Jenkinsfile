pipeline {
    agent any

    stages {
        stage('Test Start') {
            steps {
                echo 'Pipeline started successfully!'
            }
        }

        stage('Build') {
            steps {
                echo 'This is the Build stage...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running test stage...'
                sh 'echo "This is a sample test command"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage just for testing.'
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
