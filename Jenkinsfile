pipeline {
    agent {
        docker {
            image 'node:10.16-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
    stages {
        stage('Generate') {
            steps {
                sh 'npm generate'
            }
        }
    }
}
