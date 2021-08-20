pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
        post {
             always {
                 junit '**/target/*.xml'
             }
             failure {
                 mail to akshaykatrojwar@gmail.com, subject: 'The Pipeline failed :('
             }
       
        }
   }
   
}
