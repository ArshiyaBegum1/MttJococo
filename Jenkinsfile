pipeline {
    agent none

    stages {
        stage('Hello') {
            agent {label 'Jenkins-Controller'}
            steps {
                echo 'This is Jenkins Controller'
                //sh 'hostname'
                
            }
        }
        stage('maven-master') {
            agent {label 'ubuntu-new-one'}
            steps {
                echo 'Hello World from agent maven'
                sh 'mvn clean test'
                
            }
        }
    }
}
