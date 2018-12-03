pipeline {
agent none
stages {
    stage('S3download') {
      steps {
    withAWS(profile:'myProfile') {
        s3Download(file:'conf.txt', bucket:'jenkins1test', path:'/home/ilia/GitHub/s3test', force:true)
      }
    }
    }
}
                   }
