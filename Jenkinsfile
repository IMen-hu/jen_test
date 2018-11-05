pipeline {
    agent any
    stages {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
         stage('Build') {
            steps {
                sh "npm install"
            }
        }
        stage('Deploy') {
            steps {
                sh "nodejs ."
            }
        }
    }
}
