pipeline {
    agent any
    
    triggers {
        githubPush()
       // issueCommentTrigger('rebuild this')
    }
    
    options {
        // add timestamps to output
        timestamps()
    }

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

        }
                
        stage('Echo hook 11') {
            steps {
                echo 'Webhook configured properly'
            }

        }
        
    }

}



