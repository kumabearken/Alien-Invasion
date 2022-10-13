podTemplate(containers: [
    containerTemplate(name: 'python', image: 'python:3.10.7-alpine', ttyEnabled: true, command: 'cat')
  ]) {
    node(POD_LABEL) {
        container('maven') {
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
