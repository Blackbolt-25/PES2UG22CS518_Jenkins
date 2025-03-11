pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                build 'PES2UG22CS518-1'
            }
        }

        stage('Test') {
            steps {
                sh './output'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
