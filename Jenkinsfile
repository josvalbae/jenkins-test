pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo 'Test'
            }
        }

        stage('Verify branch') {
            steps {
                echo '$GIT_BRANCH'
            }
        }

        stage('Deploy to dev ?') {
            steps {
                echo 'user prompt'
            }

            input {
                message 'Deploy to dev?'
            }
        }
        
        stage('Echo hook') {
            steps {
                echo 'Webhook configured properly'
            }
        }


    }

}



