pipeline {
    agent { node { label 'workstation' } }

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

