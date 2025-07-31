pipeline {
  agent any

stages{
  stage ('checkout') {
    steps{
      checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/nallapatikrishna1/simple-java-maven-app.git']])
    }
  }
}
}
