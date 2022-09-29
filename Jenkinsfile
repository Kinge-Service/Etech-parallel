pipeline {
	agent any 
	stages{
		stage('parallel stage'){
			parallel{
				stage('parallel-job1'){
					steps{
						sh 'ps -ef'
					}
				}
				stage('parallel-job2'){
					steps{
						sh 'sudo systemctl status jenkins'
					}
				}
			}
		}
		stage('system check'){
			steps{
				echo "Welcome to Etech"
			}
		}
	}
}
