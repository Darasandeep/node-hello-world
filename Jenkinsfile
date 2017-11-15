pipeline {
    def app

    stages {
        stage('Clone') {
            checkout scm
        }

        stage('Build') {
            app = docker.build('marchie/node-hello-world')
        }

        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
