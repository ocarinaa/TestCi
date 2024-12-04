pipeline {
    agent any

    stages {
        stage('Build') { // Etapa de Build
            steps {
                echo 'Build iniciado com sucesso!' // Mensagem de build
            }
        }

        stage('Test') { // Etapa de Testes
            steps {
                echo 'Executando testes...' // Mensagem de teste
            }
        }
    }

    post { // Pós-execução
        success { // Caso o build passe
            echo 'Pipeline concluído com sucesso!' // Mensagem de sucesso
        }
        failure

