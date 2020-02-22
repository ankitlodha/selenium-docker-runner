pipeline{
	agent any
	stages{
		stage("Start Grid"){
			steps{
				sh "docker-compose up -d hub chrome firefox"
			}
		}
		stage("Run Test"){
			sh "docker-compose up book-flight-module"
		stage("Bring docker down"){
			steps{
				sh "docker-compose down"
			}
		}
	}
}
