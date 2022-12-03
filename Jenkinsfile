pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting job'
                sh "pwd"
            }
        }

        stage('checkout Wayazaexa/CplusplusAssignment') {
            steps {
                sh "pwd"
                sh "ls"
                sh "rm -rf CplusplusAssignment"
                sh "git clone https://github.com/Wayazaexa/CplusplusAssignment"
                sh "pwd"
                sh "ls"
            }
        }
        stage('compile Wayazaexa/CplusplusAssignment') {
            steps {
                sh "pwd"
                sh "ls"
                sh "cd CplusplusAssignment; make"
            }
        }
    }
}
