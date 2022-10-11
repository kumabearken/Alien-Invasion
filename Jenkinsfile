pipeline {
    agent {
        kubernetes {
            defaultContainer 'jnlp'
            yamlFile 'agentpod.yaml'
        }
    }    
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
