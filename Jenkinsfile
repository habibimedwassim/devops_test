pipeline {
    agent any
    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
    stages {
        stage('GIT Checkout') {
            steps {
                echo 'Pulling code from Git'
                git branch: 'main', 
                url: 'https://github.com/habibimedwassim/devops_test.git'
            }
        }
        stage('Building JAR') {
            steps {
                echo 'Building with Maven'
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}