pipeline {
    agent {
        label 'AGENT-1'
    }
    stages{
        stage('Build'){
            steps{
                script{
                    echo 'Build stage'
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