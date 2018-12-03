pipeline {
agent any
stages {
    stage('S3download') {
      steps {
    withAWS(profile:'myProfile') {
        s3Download(file:'conf.txt', bucket:'my-bucket', path:'/home/ilia/GitHub$
      }
    }
    }
}
}
