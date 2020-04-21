pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2',credentials:'id1YHld+y4u4gUs21ins8+HR/jZt0cBrM/vBRBf7') {

                 def identity=awsIdentity();//Log AWS credentials

                // Upload files from working directory 'dist' in your project workspace
                s3Upload(bucket:"svetojenkinsbucket", workingDir:'static', includePathPattern:'**/*');
            
            }
        }
    }
} 
