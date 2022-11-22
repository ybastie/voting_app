pipeline {
    agent { docker {
             label 'docker'
             image 'node:16.17.1-alpine' 
            } 
        }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}