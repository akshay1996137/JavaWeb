pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
    post {
         always {
              junit '**/target/*.xml'
         }
         failure {
                 mail bcc: '', body: 'failure of build', cc: '', from: '', replyTo: '', subject: 'build failed', to: 'akshaykatrojwar@gmail.com'
         }

    }

   
}
