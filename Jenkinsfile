pipeline {
    agent any
    
     
    tools {
        maven 'maven'
    }

    stages {
        stage ('checkout') {
            steps {
                git 'https://github.com/goutham1404/Project-Java-Jenkins.git'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn compile'
            }
        }
        stage ('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage ('validation') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
