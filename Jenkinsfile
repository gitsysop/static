pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
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
