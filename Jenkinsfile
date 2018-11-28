pipeline {
    agent any
    triggers {
        pollSCM('H/10 * * * *')
    }
     stages {
         stage('Build') {
             steps {
                 sh 'aca va el build'
             }
         }
         stage('Deploy') {
              steps {
                  sh 'aca va el deploy'
              }
         }
         stage('Verify') {
               steps {
                   sh 'aca va el verify'
               }
         }

     }
    post {
         success {
             echo 'El job finalizó OK! :)'
         }
         failure {
             echo 'El job rompio! :('
         }
    }
}