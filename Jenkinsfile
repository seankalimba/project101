pipeline{
    agent any
    environment{
        serverip="35.180.83.129"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                bat  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* sean@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
