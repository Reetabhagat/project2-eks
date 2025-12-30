pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t your-dockerhub-username/project2:latest .'
            }
        }

        stage('Push Image') {
            steps {
                sh 'docker push your-dockerhub-username/project2:latest'
            }
        }

        stage('Deploy to EKS using Helm') {
            steps {
                sh 'helm upgrade --install project2 ./helm-chart'
            }
        }
    }
}
