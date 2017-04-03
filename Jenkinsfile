pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
								publishLambda([awsAccessKeyId: 'ASIAJ2X6Q4MG3FPSEI3A',
															 awsRegion: 'eu-west-1',
															 awsSecretKey: '{AQAAABAAAAAwokmunbED2kyl9bgJihmqE6GzK9u/tJ+K7s9meajE02f2I4Q6ou1QHzqqJtucVZI6cQel3GGsfPoR5g6sd9iMVg==}',
															 functionARN: 'arn:aws:lambda:eu-west-1:848510910118:function:my_scheduled_lambda',
															 functionAlias: 'my_scheduled_lambda',
															 versionDescription: ''])
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

