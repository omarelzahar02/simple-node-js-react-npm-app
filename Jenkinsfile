

pipeline {
    agent {
        docker {
            image 'imbru31/node-alpine-git'
            args '-p 3000:3000 -p 5000:5000' 
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install' 
                // sh 'chown -R 109:118 "/.npm"'
            }
        }
    }
}

