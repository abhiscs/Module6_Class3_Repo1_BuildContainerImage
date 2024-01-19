pipeline {
    agent any
    stages {
        stage('dir') {
            steps {
                sh 'ls'
            }
        }     
        stage('env') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('build') {
            steps {
                sh "docker build -t springboot ."
            }
        }
    }
}