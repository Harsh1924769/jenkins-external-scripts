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
		stage('Save Output'){
			steps{
				sh 'python3 hello.py > python_output.txt'
				sh 'cat python_output.txt'
				sh 'date > date.txt'
				sh 'cat date.txt'
			}
		}
	}  	
}

