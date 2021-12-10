pipeline {
    agent any 
    stages {
        stage('clone repo and clean it') { 
            steps {
                bat "mvn clean  newmaven"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test  newmaven" 
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package  newmaven"
            }
        }
    }
}
