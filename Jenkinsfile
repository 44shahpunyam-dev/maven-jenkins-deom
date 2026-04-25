pipeline {
    agent any

    tools {
        maven 'Maven 3'
    }

    stage('Clone') {
    steps {
        git branch: 'main', url: 'https://github.com/44shahpunyam-dev/maven-jenkins-deom.git'
    }
}

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
