pipeline {
    agent any

    stages {
        stage ('fetching the code from github') {
            step {
                git branch: 'master', url: 'https://github.com/kushalsiddu/practice.git'
            }
        }

        stage ('Converting source code to executable code') {
            step {
                build: jenkinsjob
            }
        }

        stage ('Testing stage') {
            step {
                echo "This is a testing phase"
            }
        }

        stage ('Deploy stage') {
            step {
                echo "This is a deploy phase"
            }
        }
    }
}
