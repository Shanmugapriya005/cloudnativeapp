pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Shanmugapriya005/cloudnativeapp.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t cloudnativeapp .'
            }
        }

    }
}
