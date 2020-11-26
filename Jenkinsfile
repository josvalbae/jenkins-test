pipeline {
    agent any
    
    triggers {
        githubPush()
       // issueCommentTrigger('rebuild this')
    }
    
    options {
        timestamps()  // add timestamps to output
        timeout(time: 1, unit: 'HOURS') // timeout period for the Pipeline run, after which Jenkins should abort the Pipeline
        buildDiscarder(logRotator(numToKeepStr: '20'))
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



