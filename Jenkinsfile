pipeline{
    agent any
    environment{
        serverip="13.38.98.90"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh "scp -o StrictHostKeyChecking=no ${WORKSPACE}/*ubuntu@${serverip}:/var/www/html/project101"
            }
        }
    }
}
