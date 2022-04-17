pipeline {
    agent any

    stages {
        stage('test') {
            steps {
                echo 'Hello World my  name is akshay'
            }
        }
        stage('mvn test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('mvn verify') {
            steps {
                sh 'mvn verify'
            }
        }
        stage('sonar-analysis') {
            steps {
                sh 'mvn sonar:sonar'
            }
        }
        stage('mvn package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('mvn deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
        stage('deploy to tomcat'){
            steps {
               deploy contextPath: '**/webapps/', war: '**/*.war'
            }
        }

        



    }
}





















