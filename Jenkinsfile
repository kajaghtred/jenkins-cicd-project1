pipeline {
    agent any{
        
        stages {

            stage('checkout'){
                steps{
                    checkout scm
                }
            }

            stage('Install Dependencies'){
                steps {
                    bat 'python -m pip install -r requirements.txt'
                }
            }

            stage(''){
                steps {
                    bat 'pytest'
                }
            }

        }

    }
}