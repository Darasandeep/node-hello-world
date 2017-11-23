pipeline {
    agent {
        dockerfile true
    }

    stages {
        stage('Build') {
            steps {
                sh 'echo "Building artifact..."'
                sh 'echo "Storing artifact in Artifactory"'
            }
        }
        stage('Test') {
            steps {
                sh 'npm run unitTests'
                sh 'Analyse code coverage'
                sh 'npm run lint'
                sh 'npm run integrationTests'
                sh 'npm run acceptanceTests'
            }
        }
        stage('Deploy') {
            steps {
                sh 'Deploying build...'
            }
        }
    }
}
