pipeline {
    stages{
        stage('Build'){
            steps{
                script{
                    echo 'Building'
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
        }
        success {
            echo 'Build is success'
        }
        failure {
            echo 'Build is failure'
        }
    }
}