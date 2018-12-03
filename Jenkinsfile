pipeline {
    agent {
        node {
            label 'Master'
        }
    }
stages {
    stage('S3download') {
      steps {
    withAWS(credentials:'IDofAwsCredentials') {
        s3Download(file:'conf.txt', bucket:'jenkins1test', path:'/home/ilia/GitHub/s3test', force:true)
      }
    }
    }
