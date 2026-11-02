pipeline{
	agent any
	stages {
		stage('python'){
			steps{
				sh 'python3 hello.py'
				echo 'python Execution'
			}
		}
		stage('Shell'){
			steps{
				sh 'sh system_info.sh'
				echo 'Shell Execution'	
			}
		}
		stage('Verification'){
			steps{ 
				echo 'Both scripts executed successfully'
			}
		}	
	}  	
}

