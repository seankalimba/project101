pipeline{
    agent any
    environment{
        serverip="35.180.90.1"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* ubuntu@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
