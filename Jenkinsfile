pipeline {
	agent {
     docker {
        image 'laardee/serverless:latest'
        args  '-v /tmp:/tmp'
    }
	}

    stages {
        stage('Test') {
            steps {
                echo 'Testing1..'
							  sh 'uname -a'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
