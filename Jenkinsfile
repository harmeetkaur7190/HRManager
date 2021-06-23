pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "git clone https://github.com/harmeetkaur7190/HRManager.git"
            }
        }
        stage('Maven clean') {
            steps {
                bat "mvn clean"
            }
        }
        stage('Maven install') {
            steps {
                bat "mvn install"
            }
        }
        stage('Maven test') {
            steps {
                bat "mvn test"
            }
        }
        stage('Maven package') {
            steps {
                bat "mvn package"
            }
        }
    }
}