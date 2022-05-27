pipeline {
   agent { docker { image 'node:14.17.0-alpine3.13' }}
    stages {
        stage('Build') {
            steps {
                sh 'yarn build'
            }
        }
        stage('Build Docker image') {
           steps {
                sh 'yarn workspace backend build-image'
           }
        }
    }
}