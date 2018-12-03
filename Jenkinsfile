pipeline {
    agent {
        node {
            label 'Master'
        }
    }
    stages {
    stage('S3download') {
	    withAWS(profile:'myProfile')
      steps {
            s3Download(file:'conf.txt', bucket:'jenkins1test', path:'/', force:true)
        }
    }
}
}
}
