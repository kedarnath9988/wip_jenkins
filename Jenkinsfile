pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo this build stage '
            }
        }
        stage('Test') {
            steps {
                 sh 'echo this Test stage '
                 sleep 10 
            }
        }
        stage('Deploy') {
            steps {
                 sh 'echo this Deploy stage............... '
            }
        }
    }
}