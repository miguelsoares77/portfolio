pipeline {
    agent any  

    stages {

        stage('Build') {
            steps {
                script {
                    echo "building app..."
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo "testing app..."
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo "deploy app..."
                }
            }
        }

    }

    post {
        success {
            echo 'Pipeline executada com sucesso! ✅'
        }
        failure {
            echo 'Pipeline falhou! ❌'
        }
        always {
            echo 'Pipeline finalizada. Status: ${currentBuild.result}'
            cleanWs() 
        }
    }
}