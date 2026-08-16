pipeline {
    agent any

    stages {
        stage ('fetching the code from github') {
            steps {
                git branch: 'master', url: 'https://github.com/kushalsiddu/practice.git'
            }
        }

        stage ('Converting source code to executable code') {
            steps {
                build job: 'simplejob'
            }
        }

        stage ('Testing stage') {
            steps {
                echo "This is a testing phase"
            }
        }

        stage ('Deploy stage') {
            steps {
                echo "This is a deploy phase"
            }
        }
    }
}
