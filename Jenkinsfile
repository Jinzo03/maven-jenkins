pipeline {
    agent any

    stages {
        stage('Récupération du code') {
            steps {
                // Récupère automatiquement la branche configurée dans le job Jenkins
                // Récupère automatiquement la branche configurée dans le job Jenkins
                checkout scm
            }
        }
        stage('Nettoyage et Compilation Maven') {
            steps {
                // Exécute la commande Maven
                sh 'mvn clean compile'
            }
        }
    }
}
