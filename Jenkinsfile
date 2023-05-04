pipeline {
    agent any
    stages {
        stage {
            steps {
                git credentialsId: 'saurabh', url: 'https://github.com/saurabh-786-user/test-repo.git'
            }
        } 

        stage {
            steps {
                sh 'docker-compose up'
            }
        }
    }
}  
