pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3001:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                pwsh 'npm install' 
            }
        }
    }
}