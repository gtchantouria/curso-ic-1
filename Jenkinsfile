pipeline {
    agent any
    triggers {
        pollSCM('H/2 * * * *')
    }
    stages {
        stage('Build') {
         steps {
             println 'aca va el build'
             sh './gradlew build'
         }
         post{
            always{

                junit 'build/test-results/test/*.xml'
            }
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