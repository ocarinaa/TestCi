pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Clonando o repositório Git
                git 'https://github.com/ocarinaa/TestCi.git'
            }
        }
        stage('Build') {
            steps {
                // Comandos para construir o projeto
                echo 'Construindo o projeto...'
                // Exemplo de comando para rodar o build (dependendo do seu projeto)
                sh 'python setup.py install'
            }
        }
        stage('Test') {
            steps {
                // Comandos para rodar testes
                echo 'Executando os testes...'
                // Exemplo de comando para rodar testes
                sh 'python -m unittest discover'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy para produção'
                // Comando de deploy
            }
        }
    }
}
