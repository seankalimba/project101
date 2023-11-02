pipeline{
    agent any
    environment{
        serverip="13.38.98.90"
    }
    stages{
        stage('Deploy to remote server'){
            steps{
                sh -o StrictHostKeyChecking=no "scp -r ${WORKSPACE}/* sean@${serverip}:/var/www/html/project102"
            }
        }
    }
}
