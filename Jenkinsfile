pipeline {
    agent any 
    stages {
        stage('clone repo and clean it') { 
            steps {
               // bat "git clone https://github.com/nishantbodade/newmaven.git"
                bat "mvn clean -f newmaven"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test -f newmaven" 
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package -f newmaven"
            }
        }
    }
}
