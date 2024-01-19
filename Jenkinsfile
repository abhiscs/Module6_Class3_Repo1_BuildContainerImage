pipeline {
    agent any
    stages {
        stage('dir') {
            steps {
                sh 'cd Spring-Boot-Sample'
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