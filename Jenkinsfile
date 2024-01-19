pipeline {
    agent any
    stages {
        stage('env') {
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