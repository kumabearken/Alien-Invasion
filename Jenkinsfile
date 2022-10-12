pipeline {
    agent{
        kubernetes {
            label 'kubeagent'
            yaml 'agentpod.yaml'
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
