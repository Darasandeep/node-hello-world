pipeline {
    agent {
        dockerfile true
    }

    stages {
        stage('Foo') {
            steps {
                sh 'echo "Hello World!"'
            }
        }
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
