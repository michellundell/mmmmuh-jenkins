pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting job'
                sh "pwd"
            }
        }
        stage('checkout Frowsty/ticket-system') {
            steps {
                sh "pwd"
                sh "ls"
                sh "git clone https://github.com/Frowsty/ticket-system"
                //checkout([$class: 'GitSCM',branches: [[name: '*/main']],userRemoteConfigs: [[url: 'https://github.com/Frowsty/ticket-system']]])
                sh "pwd"
                sh "ls"
            }
        }
        stage('compile Frowsty/ticket-system') {
            steps {
                sh "pwd"
                sh "ls"
                sh "cd ticket-system; make"
            }
        }
    }
}
