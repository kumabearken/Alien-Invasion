pipeline {
    agent{
        kubernetes {
            label 'agent'
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
