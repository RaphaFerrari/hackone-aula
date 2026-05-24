pipeline {
    agent none
    stages {
        stage('Build') {
            agent any
            steps {
                bat 'echo comecando o build...'
                bat 'C:/Users/rapha/AppData/Local/Programs/Python/Python312/python.exe -m py_compile hello.py'
                stash(name: 'compiled-results', includes: '*.py*')
            }
        }
    }
}
