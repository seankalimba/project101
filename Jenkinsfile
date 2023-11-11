pipeline{
    agent any
    environment{
        serverip="13.36.208.55"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                bat  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* sean@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
