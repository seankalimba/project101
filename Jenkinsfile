pipeline{
    agent any
    environment{
        serverip="15.236.211.169"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                bat  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* ubuntu@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
