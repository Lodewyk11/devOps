variable = null
pipeline {
    agent any
    stages {
        stage('Some stage here') {
            steps {
                script {
                    print("Setting variable")
                    variable = "The variable value"
                }   
            }
        }

        stage('Another stage here') {
            steps {
                script {
                    print("Getting variable: " + variable)
                }   
            }
        }
    }
}