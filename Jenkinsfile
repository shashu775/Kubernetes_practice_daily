pipeline {
    agent any

    stages {

        stage('Create Nginx Pod') {
            steps {
                bat 'kubectl apply -f day1_pod\\podbasic.yaml'
            }
        }

        stage('Show Pod Status') {
            steps {
                bat 'kubectl get pods'
            }
        }
    }
}
