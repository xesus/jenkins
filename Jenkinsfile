pipeline {
    agent { docker { image 'ruby' } }
    stages {
        stage('build') {
            steps {
                sh 'ruby --version'
            }
        }
    }
    post {
        always{
            echo "This will always run."
        }
        success {
            echo "This will run only if successful."
        }
    }
}
