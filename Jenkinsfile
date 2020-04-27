pipeline {
    agent none
    stages {
        stage('Build') {
	    agent any
            steps {
                sh 'python setup.py test'
            }
        }
    }
}
