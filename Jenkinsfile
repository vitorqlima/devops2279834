pipeline {
    agent any

    stages {

        stage('Clonar Repositório') {
            steps {
                git branch: 'main', url: 'https://github.com/vitorqlima/devops2279834.git'
            }
        }
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
