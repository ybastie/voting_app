pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'docker build -t test_node .'
            }
        } 
        stage('run') {
            steps {
                sh 'docker run --dit --name node_container test_node'
            }
        }
    }
}