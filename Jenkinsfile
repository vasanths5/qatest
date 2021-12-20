pipeline {
  agent any
  stages {
    stage('initalize') {
      steps {
	    echo 'QATEST';

      }
    }
	stage('Upload to admin-center-gzip S3'){
		  when{expression { fileExists('/var/lib/jenkins/workspace/com.vtx.ui_release/dist/apps/admin-center-gzip/*.js')} }
		  steps {
	    echo 'Pass';
		  }
	}
	stage('Upload to marketplace-gzip S3'){
		  when{expression {fileExists('/var/lib/jenkins/workspace/com.vtx.ui_release/dist/apps/marketplace-gzip/*.js')} }
		  steps {
	    echo 'Pass1';
		  }

	}
    }

}

