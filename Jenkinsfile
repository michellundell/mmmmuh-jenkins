pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'; sleep 1; echo "Tjoohoo"
                echo 'baha'; sleep 1; echo "Tjoho"
            }
        }
        stage('checkout Frowsty') {
            steps {
                checkout([$class: 'GitSCM',branches: [[name: '*/main']],userRemoteConfigs: [[url: 'https://github.com/Frowsty/ticket-system']]])
                sh "pwd; ls; cd ticket-system; make"
            }
        }
    }
}
