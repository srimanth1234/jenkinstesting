pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/srimanth1234/jenkinstesting.git/'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt || true'
            }
        }

        stage('Run Unit Tests') {
            steps {
                sh 'python -m unittest discover'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Build & Tests Passed '
            }
        }
    }
}
