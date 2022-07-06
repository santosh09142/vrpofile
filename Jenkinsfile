pipeline {
    agent any
    stages {
        stage('Fetch code') {
            steps {
                git branch: 'paac', url: 'https://github.com/santosh09142/vrpofile.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
