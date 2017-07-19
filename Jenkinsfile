pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                retry(2) {
                    sh 'echo "Hello"'
                } 
                
                
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
    }
}
