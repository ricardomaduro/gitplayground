pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh '''
                    pwd
                    ls -l
                '''
                echo 'Done'
            }
        }
        stage('Test') {
            steps {
                echo 'Tests...'
                sh 'ls -l'
            }
        }
        stage('Docker') {
            agent {
                docker {
                    image 'gradle:6.7-jdk11'
                    // Run the container on the node specified at the top-level of the Pipeline, in the same workspace, rather than on a new node entirely:
                    reuseNode true
                }
            }
            steps {
                sh 'gradle --version'
            }
        }
    }
}
