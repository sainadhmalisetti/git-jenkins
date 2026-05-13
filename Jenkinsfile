pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting source code'
            }
        }

	stage('compile'){
	    steps {
		bat 'gcc demo.c'
	    }
	}
        stage('Build') {
            steps {
		bat 'a.exe'
            }
        }

    }
}