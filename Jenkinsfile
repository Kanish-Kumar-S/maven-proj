pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Kanish-Kumar-S/maven-proj.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}