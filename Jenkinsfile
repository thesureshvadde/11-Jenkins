// Jenkinsfile (Declarative Pipeline)
pipeline {
    // agent any
    agent { node { label 'AGENT-1' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post { 
        always { 
            echo 'I will always run wheather job is success or failure'
        }
        success { 
            echo 'I will run only when job is success'
        }
        failure { 
            echo 'I will run only when job is failure'
        }
    }
}