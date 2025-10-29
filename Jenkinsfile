pipeline {
    agent any
    environment {
        PYTHON = 'C:\\Users\\admin\\AppData\\Local\\Programs\\Python\\Python313\\python.exe'
    }
    stages {
        stage('Checkout code') {
            checkout scm

        }
        stage('Extract Data') {
            bat "${env.PYTHON} extract_data.py"

        }
    }
    post {
        success {
            echo "Success..........."

        }
        failure {
            echo "Failure......."
        }
        always {
            echo "Always........"

        }
    }
}
