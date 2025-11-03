pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }

        stage('Setup Environment') {
            steps {
                echo 'Installing Python...'
                sh '''
                    sudo apt-get update -y || apt-get update -y
                    sudo apt-get install -y python3 || apt-get install -y python3
                '''
                sh 'python3 --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'python3 hello.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}

