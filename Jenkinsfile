pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Construindo o código..."'
                sh 'npm install' 
            }
        }
        stage('Test') {
            steps {
                
                sh 'echo "Executando testes..."'
                sh 'npm test' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Implantando o aplicativo..."'
            }
        }
    }
    
    post {
        success {
            echo 'O pipeline foi executado com sucesso!'
        }
        failure {
            echo 'O pipeline falhou!'
        }
    }
}
