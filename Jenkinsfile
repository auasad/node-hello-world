pipeline {
    agent {
        docker {
            image 'node:alpine'
            args '-p 8090:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm start'
            }
        }
    }
}
