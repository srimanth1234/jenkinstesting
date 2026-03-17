pipeline {
    agent any

    stages {
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
