pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Simulando construcción de la aplicación...'
            }
        }
        stage('Test') {
            steps {
                echo 'Ejecutando pruebas...'
                sh 'echo "Pruebas pasadas exitosamente"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Desplegando la aplicación...'
                sh 'echo "Aplicación lista en el puerto 8081"'
            }
        }
    }
}
