pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello world"'
                sh '''
                    echo "multiline works too"
                    ls -lah
                '''
            }
        }
    }
} 
