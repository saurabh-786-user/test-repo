pipeline {
    agent any
    stages {
        stage('Pull') {
            steps {
                git credentialsId: 'saurabh', url: 'https://github.com/saurabh-786-user/test-repo.git'
            }
        } 
        stage {
            steps('Deploy') {
                sh 'docker-compose up'
            }
        }
    }
}  
