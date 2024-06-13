pipeline {
    agent { docker { image 'gcc:latest' } }
    stages {
        stage('build') {
            steps {
                sh 'gcc --version'
                sh 'gcc -o hello.c main.c'
            }
        }
        stage('test') {
            steps {
                sh './hello'
            }
        }
    }
}