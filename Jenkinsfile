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
    }
}
