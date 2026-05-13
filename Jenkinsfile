pipeline {
    agent any

    stages {

        stage('Clean') {
            steps {
                bat 'if exist demo.exe del demo.exe'
            }
        }

        stage('Compile') {
            steps {
                bat 'gcc demo.c -o demo.exe'
            }
        }

        stage('Run') {
            steps {
                bat 'demo.exe'
            }
        }

    }

    post {
        success {
            archiveArtifacts artifacts: 'demo.exe'
        }
    }
}