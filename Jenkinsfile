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
                 mail bcc: '', body: 'failure of build', cc: '', from: '', replyTo: '', subject: 'build pass', to: 'akshaykatrojwar@gmail.com'
         }

    }

   
}
