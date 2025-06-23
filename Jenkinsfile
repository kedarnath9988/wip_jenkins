pipeline {
    agent {
        label 'AGENT-01'
    }
    options {
        timeout(time: 30, unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    parameters {
        string(name: 'person', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: 'DevOps with AWS ', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }

    stages {
        stage('Build') {
            steps {
                sh 'echo this build stage '
            }
        }
        stage('Test') {
            steps {
                 sh 'echo this Test stage '
                 sh 'echo "trigger test '
                 sleep 10 
            }
        }
        stage('Deploy') {
            steps {
                 sh 'echo this Deploy stage............... '
            }
        }
       stage('print params'){
           steps {
                echo "Hello ${params.PERSON}"
                echo "Biography: ${params.BIOGRAPHY}"
                echo "Toggle: ${params.TOGGLE}"
                echo "Choice: ${params.CHOICE}"
                echo "Password: ${params.PASSWORD}"
           }

    }
    }
}

