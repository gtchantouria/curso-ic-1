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
         stage('Build') {
              steps {
                  sh 'aca va el build'
              }
         }
         stage('Deploy') {
              steps {
                  sh 'aca va el build'
              }
         }
         stage('Verify') {
               steps {
                   sh 'aca va el build'
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