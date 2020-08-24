pipeline {
	agent any
	stages {
		stage("Build") {
			steps {
				snDevOpsStep()
				echo"Build successfull"
			}
		}
		stage("Deploy UAT") {
			steps {
				snDevOpsStep()
				snDevOpsChange()
				echo"Deploy on UAT successfull"
			}
		}
		stage("Test UAT") {
			steps {
				snDevOpsStep()
				echo"Test on UAT successfull"
			}
		}
		stage("Deploy PROD") {
			steps {
				snDevOpsStep()
				snDevOpsChange()
				echo"Deploy on PROD successfull"
			}
		}
	}
}