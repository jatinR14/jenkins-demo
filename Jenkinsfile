pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/username/project.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}
