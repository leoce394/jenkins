pipeline{
    agent any
    environment{
        DIRECTORY_PATH = 'C:/Users/leoce/OneDrive/Documents/Jenkins'
        TESTING_ENVIRONMENT = '7.1C'
        PRODUCTION_ENVIRONMENT = 'Leo'
    }
    stages{
        stage('Build'){
            steps{
                echo 'Compile and package the application using Maven'
            }
        }
        stage('Test'){
            steps{
                echo 'Validate induvidual components using Jest for unit testing'
                echo 'Check that separate modules work together effectively using Supertest'
            }
        }
        stage('Code Analysis'){
            steps{
                echo 'Use SonarQube to evaluate code quality, detect bugs and ensure correct programming standards'
            }
        }
        stage('Security Scan'){
            steps{
                echo 'Use Trivy to scan container and file systems as well as repositories for vulnerabilities'
            }
        }
        stage('Deploy to Staging'){
            steps{
                echo 'Setup a Docker staging environment which acts as a pre-production server environment mimicing the live setup.'
            }
        }
        stage('Integration Tests on Staging'){
            steps{
                echo 'Run Selenium tests on the Docker staging environment to mimic to ensure stability in a sterile environment before live deployment.'
            }
        }
        stage('Deploy to Production'){
            steps{
                echo 'Deploy the now-tested application to a Docker live production environment server.'
            }
        }
    }
}
