//create pipeline to display date
pipeline {
    agent any
    stages {
        stage('GIT Checkout') {
            steps {
                echo 'Pulling code from Git'
                git branch: 'main', 
                url: 'https://github.com/habibimedwassim/devops_test.git'
            }
        }
        stage('Build') {
            steps {
                echo "Building"
                sh 'date'
            }
        }
    }
}