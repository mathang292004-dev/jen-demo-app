pipeline {
    agent any
    stages {
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run App') {
            steps {
                sh 'pm2 start app.js --name my-app || pm2 restart my-app'
            }
        }
    }
}
