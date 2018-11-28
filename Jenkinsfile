pipeline {
    agent any
    triggers {
        pollSCM('H/10 * * * *')
    }
     stages {
         stage('Build') {
             steps {
                 println 'aca va el build'
             }
         }
         stage('Deploy') {
              steps {
                  println 'aca va el deploy'
              }
         }
         stage('Verify') {
               steps {
                   println 'aca va el verify'
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