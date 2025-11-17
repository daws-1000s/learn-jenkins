pipeline {
    agent any
    options {
        ansiColor('xterm')
        timestamps()
    }
    stages {
        stage('Build'){
            steps {
                sh 'echo This is build'
            }
        }
        stage('Test'){
            steps {
                sh 'echo This is test'
            }
        }
        stage('Deploy'){
            steps {
                sh 'echo This is deploy'
                error 'pipeline failed'
            }
        }
    }
    post {
        always {
            echo "This section runs always"
        }
        success {
            echo "This section runs when pipeline is sucess"
        }
        failure {
            echo "This section runs when pipeline is failed"
        }
    }
}