pipeline{
	agent any
	stages{
	stage('Build'){
	steps{
		echo "Building the checked out project!!";
		bat label: '', script: 'build.bat'
	}
	
	}
	stage('Junit-Test'){
	steps{
		echo "Running the tests scripts !!";
	}
	
	}
	stage('Quality-gate'){
	steps{
		echo "quality checks Tests running successfully";
	}
	
	}
	}
	post{
	always{
	echo "this will run alwayss";
	}
	success{
	echo "this will work only for success";
	}
	failure{
	echo "this will work only for failure";
	}
	}
}
