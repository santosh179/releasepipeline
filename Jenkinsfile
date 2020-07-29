pipeline {
    agent any

     parameters {
            string(name: 'Greeting', defaultValue: 'Santosh', description: 'How should I greet the world?')
        }

    stages{
            stage("Checkout"){
                steps{
                    echo 'Checking out the app from GIT'
                    echo "${params.Greeting} World!"
                }
            }
            stage("Build"){
               steps{
                    echo 'Building the application using Maven'
               }
            }
            stage("Execute Unit Test Cases"){
                steps{
                    echo 'Executing Unit Test cases'
                }
            }
            stage("Deploy"){
                steps{
                    echo 'Deploying the application...'
                }
            }
    }

    post{
            always {
                echo 'Executing post always'
            }

            success {
                echo 'Executing Success'
            }

            failure {
                echo 'Executing failure'
            }

    }
}