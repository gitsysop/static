pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                sh "withAWS(region:'us-west-2,credentials:'AKIAYJ34Q7VAKC7V5JMT')", 
                    sh "s3Upload(file:'index.html', bucket:"svetojenkinsbucket", workingDir:'static', includePathPattern:'**/*')"
                   "
                }
            }
        }
    }
} 
