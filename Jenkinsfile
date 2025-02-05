pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/GaikwadAV/jenkins-pipeline.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt || echo "No dependencies to install"'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'if [ -f test_app.py ]; then python -m unittest test_app.py; else echo "No tests found"; fi'
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

