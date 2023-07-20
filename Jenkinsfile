pipeline {
    agent { node { label 'workstation' } }

    environment {
        SSH = credentials {'ssh'}
        DEMO_URL = "google.com"
    }
    options {
        ansiColor('xterm')
    }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }

    post {
        always {
            sh 'echo post'
        }
    }
}

