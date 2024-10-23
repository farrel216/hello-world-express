pipeline {
    agent {
        docker {
            image 'node:20.18.0-alpine3.20'
        }
    }
    stages {
        stage('Preparation') {
            steps {
                sh 'node --version'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}