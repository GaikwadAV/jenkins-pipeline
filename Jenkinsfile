pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/GaikwadAV/jenkins-pipeline.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python -m unittest test_app.py'
            }
        }

        stage('Build Application') {
            steps {
                sh 'echo "Building Python App..."'
            }
        }

        stage('Deploy Application') {
            steps {
                sh 'echo "Deploying Python App..."'
            }
        }
    }
}

