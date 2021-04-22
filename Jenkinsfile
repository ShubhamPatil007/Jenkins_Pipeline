pipeline {
	agent any 

	stages {
		stage('Git-Cofiguration') {
			steps {
				echo "Retreiving Git repository";
				git branch: 'main', credentialsId: 'b85d318c-dc97-485c-b2ac-8fef8b8e5ca5', url: 'https://github.com/ShubhamPatil007/Jenkins_Pipeline.git'
			}
		}

		stage('Program 1') {
			steps {
				echo "Program 1 running";
				g++ -o Program_1 Program_1.cpp
				Program_1
			}
		}

		stage('Program 2') {
			steps {
				echo "Program 2 running";
				g++ -o Program_2 Program_2.cpp
				Program_2
			}
		}

		stage('Program 3') {
			steps {
				echo "Program 3 running";
				g++ -o Program_3 Program_3.cpp
				Program_3
			}
		}
	}

}
