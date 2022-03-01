pipeline {
    agent any

    stages {
	  stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
	  stage('Verify Workspace') {
            steps {
                echo "${workspace}"
            }
        }
	  stage('List Workspace') {
            steps {
                sh (script: "ls -la '${workspace}'")
            }
        }
	  stage('Clean workspace') {
            steps {
                cleanWs()
		    echo 'Clean workspace done!'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
