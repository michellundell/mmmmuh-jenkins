pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting job'
                sh "pwd"
            }
        }
        stage('checkout') {
            steps {
                sh "pwd"
                sh "ls"
                sh "rm -rf FlightTicket"
                sh "git clone https://github.com/TobiasHoglin/FlightTicket"
                sh "pwd"
                sh "ls"
            }
        }
        stage('compile') {
            steps {
                sh "pwd"
                sh "ls"
                sh "cd FlightTicket; make"
            }
        }
    }
}
