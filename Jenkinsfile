pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/srimanth1234/jenkinstesting.git'
            }
        }

        stage('Run Unit Tests') {
            steps {
                bat 'python -m unittest discover'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Build & Tests Passed ✅'
            }
        }
    }
}
