pipeline {
    agent any 

    options{
        timeout(time: 30, unit: 'minutes')
        disableConcurrentBuilds()
    }

    stages{
        stage('Dev'){
            steps{
                echo 'this is dev stage'
            }
        }
        stage('test'){
            steps{
                echo 'this is test stage'
                sleep 30 
            }
        }
        stage('deploy'){
            steps{
                echo 'thic is deploy stage'
            }
        }
    }
}