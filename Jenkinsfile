pipeline {
    agent any 
    stages {
        stage('clone repo and clean it') { 
            steps {
                bat "mvn clean  "
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test  " 
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package  "
            }
        }
    }
}
