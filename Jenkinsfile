pipeline {
    podTemplate(containers: [
        containerTemplate(
            name: 'python', 
            image: 'python:latest', 
            command: 'sleep', 
            args: '30d')
    ]){
        stages {
            node(POD_LABEL) {
                stage('version') {
                    container('python'){
                        steps {
                            sh 'python3 --version'
                        }
                    }
                }
                stage('hi'){
                    container('python'){
                        steps{
                            sh 'python3 hi.py'
                        }
                    }
                }
            }
        }
    }
}
