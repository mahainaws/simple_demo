pipeline {
	agent any
	stages {
		stage("Clone") {
			steps {
				echo 'Code is being pulled from GitHub'
				sleep 1
				echo 'Cloning is Completed'
			}
		}
		
		stage("Compile") {
			steps {
				echo 'Code compilation is in Progress'
				sleep 1
				echo 'Compilation is Completed..'
			}
		}
		stage("Deploy to Dev") {
			steps {
				echo 'Dev deploy is in Progress'
				sh 'scp -i /home/ec2-user/.ssh/id_rsa index.html ec2-user@172.31.15.106:/opt/tomcat/webapps/demo'
			}
		}
}
}
