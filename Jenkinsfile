pipeline {
    agent {
        docker {
            image 'python:3.10'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Python script...'
                sh 'python3 hello.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment successful!'
            }
        }
    }
}

