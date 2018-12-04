pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'python:2.7'
                }
            }
            steps {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
    }
}
