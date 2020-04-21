pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2',credentials:'AKIAYJ34Q7VAKC7V5JMT')

                 //def identity=awsIdentity();//Log AWS credentials

                // Upload files from working directory 'dist' in your project workspace
                s3Upload(bucket:"svetojenkinsbucket", workingDir:'static', includePathPattern:'**/*');
            
            }
        }
    }
} 
