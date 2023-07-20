pipeline {
    agent { node { label 'workstation' } }

    environment {
        SSH = credentials {'ssh'}
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

