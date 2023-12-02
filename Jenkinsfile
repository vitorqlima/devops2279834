pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Exemplo de passos para construir o código
                sh 'echo "Construindo o código..."'
                sh 'npm install' // Comando para instalar dependências, se for um projeto Node.js
            }
        }
        stage('Test') {
            steps {
                // Exemplo de passos para executar testes
                sh 'echo "Executando testes..."'
                sh 'npm test' // Comando para executar testes, se for um projeto Node.js
            }
        }
        stage('Deploy') {
            steps {
                // Exemplo de passos para implantar o aplicativo
                sh 'echo "Implantando o aplicativo..."'
                sh 'npm run deploy' // Comando para implantar, se for um projeto Node.js
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
