pipeline{
    agent any
    environment{
        serverip="13.38.98.90"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh "scp -r ${WORKSPACE}/* root@${serverip}:/var/www/html/project101"
            }
        }
    }
}
