pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/pooja1923/MavenCalculator_Jenkins.git'
            }
        }
        stage('Clean') {
            steps {
                bat 'mvn clean'
            }
        }
        stage('Compile') {
            steps {
                bat 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
