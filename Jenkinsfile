pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Construyendo la imagen...'
                sh 'docker build -t mi-app-jenkins .'
            }
        }
        stage('Test') {
            steps {
                echo 'Ejecutando pruebas...'
                sh 'node -v'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Desplegando la aplicación...'
                sh 'docker rm -f mi-app-jenkins-container || true'
                sh 'docker run -d -p 8081:3000 --name mi-app-jenkins-container mi-app-jenkins'
            }
        }
    }
}
