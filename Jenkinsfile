pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "npm install"
            }
        }
        stage('Deploy') {
            steps {
                sh "nodejs . 2> null"
            }
        }
    }
}