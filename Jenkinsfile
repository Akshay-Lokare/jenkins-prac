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
            }
        }

        stage("Test") {
            steps {
                echo '${%JAVA_HOME%}'
                echo 'Application testing started'
            }
        }

        stage("Deploy") {
            steps {
                echo 'Application deployment started'
            }
        }

    }
}