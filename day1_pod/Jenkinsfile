pipeline {
    agent any

    stages {

        stage('Checkout Code from GitHub') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/shashu775/Kubernetes_practice_daily.git'
            }
        }

        stage('Apply Kubernetes Pod') {
            steps {
                sh 'kubectl apply -f k8s/nginx-pod.yaml'
            }
        }

        stage('Show Pod Status') {
            steps {
                sh 'kubectl get pods'
            }
        }
    }
}
