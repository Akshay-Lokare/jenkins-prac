pipeline {
    agent any
    stages {
        stage('Build'){
           steps {
             bat 'echo Building 1 the app...'
             bat 'echo Building 2 the app...'
             bat 'echo Building 3 the app...'
           }
        }
        stage('Test'){
           steps {
             bat 'echo Testing the app...'
           }
        }
        stage('Deploy'){
           steps {
             bat 'echo Deploying the app...'
           }
        }
    }
}