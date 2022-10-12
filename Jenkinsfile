pipeline {
    agent {
        kubernetes {
            yamlFile 'agentpod.yaml'
        }
    }
    stages {
        stage('version') {
            steps {
                sh 'python3 --version'
            }
        }
        stage('hi'){
            steps{
                sh 'python3 hi.py'   
            }
        }
    }
}
 
