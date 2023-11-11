pipeline{
    agent any
    environment{
        serverip="13.37.242.178"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh  "scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/* ubuntu@${serverip}:/var/www/html/projectX"
            }
        }
    }
}
