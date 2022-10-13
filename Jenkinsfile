podTemplate(yaml: 'agentpod.yaml', cloud: 'kubernetes'){
    node(POD_LABEL) {
        container('python') {
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
    }
}
