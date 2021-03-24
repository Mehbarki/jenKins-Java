pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Mehbarki/jenKins-Java.git'
            }
        }
        stage('build') {
            steps {
                sh "javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "java Main"
            }
        }
    }
}
