pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t trend-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker tag trend-app sandhyamanikanta/trend-app:v1'
                sh 'docker push sandhyamanikanta/trend-app:v1'
            }
        }

        stage('Deploy Kubernetes') {
            steps {
                sh 'kubectl apply -f deployment.yaml'
                sh 'kubectl apply -f service.yaml'
            }
        }
    }
}
