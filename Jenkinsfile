pipeline {
    agent any

    tools {
        jdk 'Java21'
    }

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/lailawaleed/Cloud-Computing-Task4-.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
        stage('Run Unit Tests') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
