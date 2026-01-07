pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout([
                    $class: 'GitSCM',
                    branches: [[name: 'main']],
                    userRemoteConfigs: [[
                        url: 'https://github.com/Jdcharls/Documents.git',
                        credentialsId: 'c206c6da-e32a-4feb-88a2-8b5880f9bda0'
                    ]]
                ])
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage...'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage...'
            }
        }
    }
}
