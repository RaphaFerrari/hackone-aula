pipeline {
    agent none
    stages {
        stage('Build') {
            agent any
            steps {
                bat 'echo comecando o build...'
                bat 'python3 -m py_compile hollo.py'
                stash(name: 'compiled-results', includes: '*.py*')
            }
        }
    }
}
