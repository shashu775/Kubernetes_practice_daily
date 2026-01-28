pipeline {
    agent any

    stages {

        stage('Create Nginx Pod') {
            steps {
                bat 'kubectl apply -f k8s\\nginx-pod.yaml'
            }
        }

        stage('Show Pod Status') {
            steps {
                bat 'kubectl get pods'
            }
        }
    }
}
