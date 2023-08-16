pipeline {
    agent {
        docker {
            image 'node:18.17.1-alpine3.18' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
                sh 'chown -R 109:118 "/.npm"'
            }
        }
    }
}

