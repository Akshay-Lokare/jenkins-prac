pipeline {
    agent any

    stages {

        stage("Checkout") {
            steps {
                echo "Source code checkout started"
            }
        }

        stage("Build") {
            tools {
                jdk 'JAVA-11'
            }
            steps {
                echo "Application build started"
                bat 'java -version'
                bat 'javac -version'
            }
        }

        stage("Test") {
            steps {
                echo 'Application testing started'
                bat 'echo JAVA_HOME=%JAVA_HOME%'
            }
        }

        stage("Deploy") {
            steps {
                echo 'Application deployment started'
            }
        }

    }
}