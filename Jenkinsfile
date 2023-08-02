pipeline {
  agent {
    label {
	 label 'slave1'
	  customWorkspace "/mnt/multibranch-on-slave1/"
	       }
		 }
	stages {
	 stage ('clean Workspace') {
	  steps {
	     cleanWs ()
		    }
		  }
	  stage ('23Q2 on master') {
	   steps {
	     sh "sudo git clone https://github.com/keshavkale123/multibranch-on-slave.git -b 23Q2"
		   sh "sudo cp -r /mnt/multibranch-on-slave1/multibranch-on-slave/index.html /var/www/html/"
		   sh "sudo chmod -R 777 /var/www/html/"
		      }
			 }
		}
	}
	
		 
