pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }     
        stage('Build') {
            steps {
                // sh 'mvn --version'
                sh "docker build -t springboot ."
            }
        }
    }
}