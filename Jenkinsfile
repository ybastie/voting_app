pipeline {
    agent { label "maître" }
    stages {
        stage('build') {
            steps {
                sh 'docker build -t test_node .'
            }
        } 
        stage('run') {
            steps {
                sh 'docker run --dit node_container test_node'
            }
        }
    }
}