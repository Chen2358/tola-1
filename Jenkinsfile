pipeline {
    agent none
    stages {
        stage('Test') {
	    agent{
		docker{
			image 'python:2-alpine'
		}
	    }
            steps {
                sh 'python setup.py test'
            }
	    post {
		always {
			junit 'test-reports/results.xml'		
		}
	    }
        }
    }
}
