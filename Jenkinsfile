pipeline {
  agent any
  stages {
    stage('initalize') {
      steps {
	    echo 'QATEST';

      }
    }
	stage('Upload to admin-center-gzip S3'){
		  when{expression { fileExists('/var/lib/jenkins/workspace/DBBackUp')} }
		  steps {
	    echo 'Pass';
		  }
	}
	stage('Upload to marketplace-gzip S3'){
		  when{expression {fileExists('/var/lib/jenkins/workspace/DBBackUp')} }
		  steps {
	    echo 'Pass1';
		  }

	}
    }

}

