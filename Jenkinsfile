pipeline {
    agent any
    stages {
         stage('Pull code') {
            steps {
                sh 'git credentialsId: 'saurabh', url: 'https://github.com/saurabh-786-user/test-repo.git'
            }
         } 
        stage('Build Project Develop') {
            when {
                branch 'master'
            }
            steps {
                sh 'docker compose up  '
            }
        }
    }
}
