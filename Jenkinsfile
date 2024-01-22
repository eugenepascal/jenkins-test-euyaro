pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code depuis le repository Git sur une branche spécifique
                git branch: 'main', url: 'https://github.com/eugenepascal/jenkins-test-euyaro.git'
            }
        }
        stage('Test') {
            steps {
                // Exécuter les tests Python
                sh 'python -m unittest test_main.py'
            }
        }
    }
}
