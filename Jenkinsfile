pipeline {
    agent {
        dockerfile true
    }

    stages {
        stage('Foo') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
