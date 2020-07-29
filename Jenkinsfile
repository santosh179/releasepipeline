pipeline {
    agent any
    stages{
            stage("Checkout"){
                steps{
                    echo 'Checking out the app from GIT'
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
}