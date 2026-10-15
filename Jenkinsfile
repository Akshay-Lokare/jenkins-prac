pipeline {
    agent any

    stages {
        stage ("Show Parameters") {
            steps {
                echo 'Select Env: ${params.Environment}'
                echo 'Run Tests: ${params.RunTest}'
            }
        }
        stage ("Build") {
            echo "Building the app"
        }
        stage ("Test") {
            when {
                expression {
                    params.RunTest == true
                }
            }
            steps {
                bat 'echo Testing the app'
            }
        }
        stage ("Deploy") {
            steps {
                bat 'echo Deploying the app'
            }
        }
    }

}