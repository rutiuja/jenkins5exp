
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/rutiuja/jenkins5exp.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running...'
                bat 'java HelloWorld'
            }
        }
    }
}
