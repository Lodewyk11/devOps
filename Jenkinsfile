variable = null
pipeline {
    agent any
    parameters {
        choice(name: "Choice", choices: ["one", "two", "three"])
    }

    stages {
        stage("Getting the choice") {
            steps {
                script {
                    print("Setting variable")
                    variable = parameters.Choice
                }   
            }
        }

        stage("Mapping the choice") {
            steps {
                script {
                    switch(variable) {
                        case "one":
                            print("1")
                            break;
                        case "two":
                            print("1")
                            break;
                        case "three":
                            print("1")
                            break;
                        default:
                            print("I got nuffin...")
                            break;        
                    }
                    print("Getting variable: " + variable)
                }   
            }
        }


    }
}