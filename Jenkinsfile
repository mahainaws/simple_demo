pipeline {
	agent any
	stages {
		stage("Clone") {
			steps {
				echo 'Code is being pulled from GitHub'
				sleep 6
				echo 'Cloning is Completed'
			}
		}
		
		stage("Compile") {
			steps {
				echo 'Code compilation is in Progress'
				sleep 5
				echo 'Compilation is Completed'
			}
		}
		stage("Deploy to Dev") {
			steps {
				echo 'Dev deploy is in Progress'
				sh 'cp index.html /opt/tomcat/webapps/demo'
			}
		}
}
}