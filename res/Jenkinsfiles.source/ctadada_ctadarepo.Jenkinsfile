
pipeline {
//    agent { docker { image 'python:3.5.1' } }
    agent any
    stages {
/*        stage('build') {
            steps {
                sh 'python3 --version'
            }
        } */
        stage('Test') {
            steps {
//                sh 'echo "Fail!"; exit 1'
                sh 'echo "Hahaha!"'
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
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
