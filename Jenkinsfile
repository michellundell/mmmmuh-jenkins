pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting job'
            }
        }
        stage('checkout Frowsty/ticket-system') {
            steps {
                checkout([$class: 'GitSCM',branches: [[name: '*/main']],userRemoteConfigs: [[url: 'https://github.com/Frowsty/ticket-system']]])
            }
        }
        stage('compile Frowsty/ticket-system') {
            steps {
                sh "pwd; ls; cd ticket-system; make"
            }
        }
    }
}
