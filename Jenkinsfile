pipeline {
    agent any 
    stages {
        stage('slave2'){
            steps {
                build 'slave2'
            }
        } 
        stage('compile') { 
            steps {
                sh "mvn compile"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('package'){
            steps {
                sh "mvn package"
            }
        }
    }
}
