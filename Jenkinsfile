pipeline {
    agent any

    stages {

        stage('Fetching the code from GitHub') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/kushalsiddu/practice.git''
            }
        }

        stage('Converting source code to executable code') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Testing stage') {
            steps {
                echo 'This is a testing phase'
            }
        }

        stage('Deploy stage') {
            steps {
                echo 'This is a deploy phase'
            }
        }
    }
