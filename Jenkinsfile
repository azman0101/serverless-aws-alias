pipeline {
	agent {
     docker {
        image 'azman0101/serverless:latest'
        args  '-v /tmp:/tmp'
    }
	}

    stages {
        stage('Test') {
            steps {
                echo 'Testing1..'
							  sh 'uname -a'
								sh 'pwd'
								sh 'ls -lah'
							  sh 'node --version'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
