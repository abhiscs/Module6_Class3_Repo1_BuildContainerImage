pipeline {
    agent any
    stages {

        stage('env') {
            steps{
                sh 'cd Spring-Boot-Sample'
            }
        }     
        stage('env') {
            steps{
                sh 'mvn clean install'
            }
        }
        stage('build') {
            steps {
                // sh 'mvn --version'
                sh "docker build -t springboot ."
            }
        }
    }
}