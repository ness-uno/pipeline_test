pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
              echo 'Clone....'

              checkout scm
            }
        }
        stage('Test') {
            steps {
              echo 'Test....'
              sh "./docker.sh"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sleep 460
            }
        }
    }
}
