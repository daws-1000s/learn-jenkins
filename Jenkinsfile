pipeline {
    agent any 
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
                s 'echo This is deploy'
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