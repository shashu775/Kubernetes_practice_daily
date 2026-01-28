pipeline {
    agent any

    stages {

        stage('Create Pod from Repo YAML') {
            steps {
                bat 'kubectl apply -f day1_pod\\podbasic.yaml --validate=false'
            }
        }

        stage('Verify Pod') {
            steps {
                bat 'kubectl get pods'
            }
        }
    }
}
