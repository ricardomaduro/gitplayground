pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh '''
                    rm -rf gitplayground
                    git clone https://github.com/ricardomaduro/gitplayground.git
                    cd gitplayground
                    ls -l
                '''
                echo 'Done'
            }
        }
    }
}
