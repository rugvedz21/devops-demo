pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/rugvedz21/devops-demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'ls -la'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'test -f index.html && echo index.html found'
            }
        }
    }
}
