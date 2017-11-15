pipeline {
    agent {
        docker 'marchie-nodehelloworld:1'
    }
    stages {
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
