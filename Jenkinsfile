pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'Hello World'
<<<<<<< HEAD
	}
    }
    stage('Upload to AWS') {
      steps {
        withAWS(region:'ap-southeast-1',credentials:'aws-static') {
          //upload file into s3-bucket
          s3Upload(file:'index.html', bucket:'udacity-jenkins-example', path:'/index.html')
	}
      }
    }
=======
        sh '''
           echo "multipleline "
           ls -lah
        '''
      }
    }

>>>>>>> b2a37ece8de5dcb0a6e066155b54a7f3cf5e2e50
  }
}