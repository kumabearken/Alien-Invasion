pipeline {
    agent {
        kubernetes {
            yamlFile 'agentpod.yaml'  // path to the pod definition relative to the root of our project 
        }
    }
    stages {
        stage('version') {
            steps {
                sh 'python3 --version'
            }
        }
        agent any
        stage('hi'){
            steps{
                sh 'python3 hi.py'   
            }
        }
    }
}
