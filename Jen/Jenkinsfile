pipeline {
    agent {
        label 'slave'
    }
    tools {
        maven 'maven' // Use the name configured in Jenkins
    }
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/summu97/monolythic-project.git'
            }
        }
        stage('package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
