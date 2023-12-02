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
                /
                sh 'echo "Implantando o aplicativo..."'
            }
        }
    }
    
    post {
        success {
            // Ações a serem executadas se o pipeline for bem-sucedido
            echo 'O pipeline foi executado com sucesso!'
            // Pode adicionar notificações ou outras ações aqui
        }
        failure {
            // Ações a serem executadas se o pipeline falhar
            echo 'O pipeline falhou!'
            // Pode adicionar notificações ou outras ações aqui
        }
    }
}
