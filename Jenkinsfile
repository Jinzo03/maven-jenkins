pipeline {
    agent any

    triggers {
        // Vérifie le dépôt Git toutes les minutes pour détecter un nouveau push
        pollSCM('* * * * *')
    }

    stages {
        stage('Récupération du code source') {
            steps {
                // Extrait automatiquement le code depuis le dépôt Git configuré dans le job
                checkout scm
            }
        }

        stage('Affichage de la date système') {
            steps {
                // Affiche la date système de l'agent d'exécution
                sh 'date'
            }
        }
    }
}