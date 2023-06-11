pipeline{
    agent any
    environment {
        DIRECTORY_PATH = "https://github.com/dkrunal31/sit323_737-2023-t1-prac2p.git"
        TESTING_ENVIRONMENT = "test-environment"
        PRODUCTION_ENVIRONMENT = "your-name-environment"
    }

    stages{
        stage('Build'){
            steps{
                echo "Fetch the source code from the directory path ${env.DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artifacts"
            }   
        }
        stage('Test'){
            steps{
                echo "Unit tests"
                echo "Integration tests"
            }   
        }
        stage('Code Quality Check'){
            steps{
                echo "Check the quality of the code"
            }   
        }
        stage('Deploy'){
            steps{
                echo "Deploy the application to a testing environment specified by the environment variable ${env.TESTING_ENVIRONMENT}"
            }   
        }
        stage('Approval'){
            steps{
                echo "Approval started, waiting for 10 seconds to simulate manual approval"
                sleep 10
            }   
        }
        stage('Deploy to Production'){
            steps{
                echo "Deploy the code to the production environment using the environment variable specifying the environment name ${env.PRODUCTION_ENVIRONMENT}"
            }   
        }
        stage('Poll Feature Test 2'){
            steps{
                echo "Yeyy, Poll is working again"
            }   
        }
    }
}
