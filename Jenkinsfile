pipeline {
    agent any
    
    tools {
        maven 'maven'
    }
    stages {
        stage('Build stage') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
    post {
        success {
            echo "success build"
        }
        failure {
            echo "failure build"
        }
    }
}
