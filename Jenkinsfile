pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python setup.py test'
            }
        }
    }
    post {
        always {
            junit 'build/reports/**/*.xml'
        }
    }
}
