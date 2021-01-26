pipeline {
	agent any
	stages {
		stage("build") {
				steps {
					echo "STARTING BUILD"

					sh 'docker build -t "flaskapp:v1" .'
					
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
