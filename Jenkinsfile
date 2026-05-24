pipeline {
    agent none
    stages {
        stage('Build') {
            agent any
            steps {
                sh 'echo comecando o build...'
                sh 'python3 -m py_compile hollo.py'
                stash(name: 'compiled-results', includes: '*.py*')
            }
        }
    }
}
