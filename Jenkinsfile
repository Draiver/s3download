pipeline {
    agent {
        node {
            label 'Master'
        }
    }
    options {
	withAWS(profile:'myProfile')
stages {
    stage('S3download') {
      steps {
            s3Download(file:'conf.txt', bucket:'jenkins1test', path:'/', force:true)
        }
    }
}
}
