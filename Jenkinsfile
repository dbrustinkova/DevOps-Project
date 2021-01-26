pipeline {
	agent any
	stages {
		stage("build") {
				steps {
					echo "STARTING BUILD"

					sh 'docker build -t "flaskapp:$GIT_COMMIT" .'
					
					echo "BUILD WAS SUCCESSFUL"
				}
		}
		stage("test") {
				steps {
					echo "STARTING TEST"
				}
		}
		stage("deploy") {
				steps {
					echo "STARTING DEPLOY"
				}
		}
	}
}
