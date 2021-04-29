pipeline {
	agent any 

	stages {
		stage('Git-Cofiguration') {
			steps {
				echo "Retreiving Git repository";
				git branch: 'main', credentialsId: 'b85d318c-dc97-485c-b2ac-8fef8b8e5ca5', url: 'https://github.com/ShubhamPatil007/Jenkins_Pipeline.git'
				
				def dockerHome = tool 'docker'
       				env.PATH = "${dockerHome}/bin:${env.PATH}"
			}
		}

		stage('Program 1') {
			steps {
				echo "Program 1 running";
				bat 'g++ -o Program_1 Program_1.cpp'
			}
		}

		stage('Program 2') {
			steps {
				echo "Program 2 running";
			}
		}

		stage('Program 3') {
			steps {
				echo "Program 3 running";
			}
		}
	}
}
