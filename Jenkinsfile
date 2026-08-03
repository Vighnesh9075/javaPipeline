pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }

        stage('compile') {
            steps {
                bat 'javac Hello.java'
            }
        }
        stage('clone repository') {
            steps {
                git branch: 'main', credentialsId: '401c5ce8-31a0-44c2-9d79-1cd05565b83d', url: 'https://github.com/Vighnesh9075/javaPipeline.git'
            }
        }

        stage('run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}
