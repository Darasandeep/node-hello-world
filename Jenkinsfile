pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                app = docker.build('marchie/node-hello-world')
            }
        }

        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
