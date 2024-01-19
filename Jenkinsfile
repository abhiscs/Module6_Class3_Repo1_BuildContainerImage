pipeline {
    agent any
    stages { 
        stage('env') {
            steps {
                sh 'mvn clean install -f ./Spring-Boot-Sample/pom.xml'
            }
        }
        stage('build') {
            steps {
                sh "docker build -t springboot ./Spring-Boot-Sample/"
            }
        }
    }
}