pipeline {
    agent none
    stages {
        stage('Build') {
            steps {
                sh 'python setup.py test'
            }
        }
    }
}
