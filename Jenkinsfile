pipeline {
	agent {
     docker {
        image 'laardee/serverless:latest'
        label 'my-defined-label'
        args  '-v /tmp:/tmp'
    }
	}

    stages {
        stage('Test') {
            steps {
                echo 'Testing1..'
							  uname -a
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
