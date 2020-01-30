pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
	sh 'tidy -q -e *.html'
	}
    }
    stage('Upload to AWS') {
      steps {
        withAWS(region:'ap-southeast-1',credentials:'aws-static') {
          //upload file into s3-bucket
          s3Upload(file:'index.html', bucket:'udacity-jenkins-example', path:'index.html')
	}
      }
    }
  }
}
