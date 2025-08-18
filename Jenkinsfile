pipeline {
    agent {
        label 'AGENT-1'
    }
    environment {
        COURSE = 'Devops with Jenkins'
    }
    options {
        timeout(time: 30, unit: 'MINUTES') 
        disableConcurrentBuilds()
    }
    stages{
        stage('Build'){
            steps{
                script{
                    sh """
                    echo 'Build stage'
                    sleep 10
                    env
                    """
                }
            }
        }
        stage('Test'){
            steps{
                script{
                    echo 'Testing'
                }
            }
        }
        stage('Deploy'){
            steps{
                script{
                    echo 'Deploying'
                }
            }
        }
    }
    post {
        always {
            echo 'I will say hello again'
            deleteDir()
        }
        success {
            echo 'Build is success'
        }
        failure {
            echo 'Build is failure'
        }
    }
}