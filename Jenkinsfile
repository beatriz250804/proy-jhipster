pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/beatriz250804/proy-jhipster.git'
            }
        }

        stage('Build') {
            bat 'mvnw clean install'
        }

        stage('Test') {
            bat 'mvnw test'
        }
    }
}
