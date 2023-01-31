pipeline {

	agent {
				label {
				
				
				label "built-in"
				customWorkspace "/mnt/project"
				
				}
	}
	
	stages {
		
			stage ('git-clone') {
				
					steps {     
					            sh "rm -rf *"
								sh "sudo yum install git -y"
								sh "sudo yum install httpd -y"
								sh "git clone https://github.com/avadhutpatils/test.git"
								sh "cd test && sudo cp -r index.html /var/www/html/"
								sh "sudo chmod -R 777 /var/www/html"
								sh "sudo service httpd start"
					}
			
			}
			}
			}
