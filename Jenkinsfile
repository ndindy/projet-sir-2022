pipeline {
	agent any
	tools {
		maven '3.6.3'
	}

	stages {
		stage('Source') {
			steps{
				git branch: 'master', url: 'https://github.com/ndindy/projet-sir-2022.git'
		}

		stage('Build') {
			steps {
				bat 'mvn clean package'
			}
		}
	}