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

        stage('run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}
