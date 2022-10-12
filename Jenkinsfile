def AGENT_LABEL = null

pipeline {
    stages {
            agent any
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
