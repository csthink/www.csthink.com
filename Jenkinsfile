pipeline {
  agent {
        docker {
            image 'node:10.16-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'npm config set registry https://registry.npm.taobao.org'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Generate') {
          when {
              expression {
                currentBuild.result == null || currentBuild.result == 'SUCCESS'
              }
          }
          steps {
              sh 'npm run generate'
          }
        }
    }
}
