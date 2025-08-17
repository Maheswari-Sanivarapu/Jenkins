pipeline {
    agent {
        label 'AGENT-1'
    }
    environment {
        COURSE = 'Devops with Jenkins'
    }
    stages{
        stage('Build'){
            steps{
                script{
                    sh """
                    echo 'Building'
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