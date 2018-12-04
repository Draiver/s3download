pipeline {
agent any
stages {
    stage('S3download') {
      steps {
    withAWS(credentials:'nameOfSystemCredentials') {
        s3Download(file:'conf.txt', bucket:'my-bucket', path:'/home/ilia/GitHub/s3test/conf.txt', force:true)
      }
    }
    }
}
}

