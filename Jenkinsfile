pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/jatinR14/jenkins-demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing Stage'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploy Stage'
            }
        }

    }
}
