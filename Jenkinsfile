pipeline {
  agent {
    label {
	 label 'master'
	  customWorkspace "/mnt/multibranch-on-slave/"
	       }
		 }
	stages {
	 stage ('clean Workspace') {
	  steps {
	     cleanWs ()
		    }
		  }
	  stage ('23Q1 on master') {
	   steps {
	     sh "git clone https://github.com/keshavkale123/multibranch-on-slave.git -b 23Q1"
		   sh " cp -r /mnt/multibranch-on-slave/multibranch-on-slave/index.html /var/www/html/"
		   sh "chmod -R 777 /var/www/html/"
		      }
			 }
		}
	}
