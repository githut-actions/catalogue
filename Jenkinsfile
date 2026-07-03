pipeline {
    agent {
        label 'AGENT-1'
    }

    options {
        timeout(time: 1, unit: 'MINUTES')
        disableConcurrentBuilds()
    }

    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                        echo "hello build"
                        
                    """
                }
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
    }

    post {
        always {
            echo 'I will always say hello'
            deleteDir()
        }

        success {
            echo 'hello success'
        }

        failure {
            echo 'hello failure'
        }
    }
}