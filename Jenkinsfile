pipeline {
    agent {
        docker {
            image 'node:14.20.0-bullseye' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo npm install -g node-gyp'
                sh 'npm install' 
            }
        }
    }
}