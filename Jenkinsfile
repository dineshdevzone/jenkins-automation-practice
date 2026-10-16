pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building HTML application'
                sh 'ls -l'
            }
        }

        stage('Test') {
            steps {
                sh 'test -f index.html'
                echo 'HTML file check passed!'
            }
        }
    }
}
