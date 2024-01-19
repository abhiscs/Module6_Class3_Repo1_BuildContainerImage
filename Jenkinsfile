pipeline {
    agent { 
        node {
            label 'any'
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }    
    post {
        success {
            echo 'Job completed successfully'
        }
        failure {
            echo 'Job failed'
        }
    }
}
