variable = null
pipeline {
    agent any
    parameters {
        choice(name: "Choice", choices: ["one", "two", "three"], description: 'Pick something')
    }

    stages {
        stage("Getting the choice") {
            steps {
                script {
                    print("Setting variable")
                    variable = params.Choice
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
                            print("2")
                            break;
                        case "three":
                            print("3")
                            break;
                        default:
                            print("I got nuffin...")
                            break;        
                    }
                }   
            }
        }


    }
}