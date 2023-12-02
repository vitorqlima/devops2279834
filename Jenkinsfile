pipeline {
    agent any

    stages {
        stage('Construir') {
            steps {
                sh 'npm install'
                sh 'npm build'  
            }
        }
        stage('Testar') {
            steps {
                sh 'npm test'     
            }
        }
    }
}
