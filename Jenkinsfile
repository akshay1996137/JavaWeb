pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World my  name is akshay'
            }
        }
        stage('mvn test') {
            steps {
                sh mvn test
            }
        }
        stage('mvn compile') {
            steps {
                sh mvn compile
            }
        }
        stage('mvn verify') {
            steps {
                sh mvn verify
            }
        }
    }
}





















