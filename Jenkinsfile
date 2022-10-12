def AGENT_LABEL = null

pipeline {
    agent{
        kubernetes {
            label "${AGENT_LABEL}"
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
