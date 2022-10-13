podTemplate(containers: [
    containerTemplate(
        name: 'python', 
        image: 'python:latest', 
        command: 'sleep', 
        args: '30d')
  ]) {

    node(POD_LABEL) {
        stage('Build a python project') {
            container('python') {
                stage('Shell Execution') {
                    checkout scm
                    sh 'python Alien-Invasion/AlienInvasion/venv/Scripts/AlienInvasion.py'
                }
            }
        }

    }
}
