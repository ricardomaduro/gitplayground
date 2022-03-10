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
    }
}
