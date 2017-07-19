pipeline {
    agent docker { image 'node:7-alpine' }
    stages {
        stage('build') {
            steps {
                retry(2) {
                    sh 'npm --version'
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
