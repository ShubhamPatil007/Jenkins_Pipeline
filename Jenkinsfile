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
				bat "Program_1.bat";
			}
		}

		stage('Program 2') {
			steps {
				echo "Program 2 running";
				bat "Program_2.bat";
			}
		}

		stage('Program 3') {
			steps {
				echo "Program 3 running";
				bat "Program_3.bat";
			}
		}
	}

}
