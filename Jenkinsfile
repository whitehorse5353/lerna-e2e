pipeline {
    agent {
        docker {
            image 'node:10.16.0-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
            steps {
                sh 'npm run release'
            }
        }

    }
}
