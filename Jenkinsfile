pipeline{
    agent any
    environment{
        serverip="15.188.185.200"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* sean@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
