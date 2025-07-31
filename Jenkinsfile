pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                  checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/nallapatikrishna1/simple-java-maven-app.git']])

            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'mvn clean install'
            }
        }
    }
}
