pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // sh 'mvn --version'
                sh "docker build -t springboot ."
            }
        }
    }
}