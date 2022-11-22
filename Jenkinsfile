pipeline {
    agent { label "linux" }
    stages {
        stage('build') {
            steps {
                sh 'docker build -t test_node .'
            }
        }
    }
    stages {
        stage('run') {
            steps {
                sh 'docker run --dit node_container test_node'
            }
        }
    }
}