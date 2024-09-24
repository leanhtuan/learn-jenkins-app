pipeline {
    agent any

    stages {
        stage('Hello') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps {
                sh 'echo "Hello from Jenkins"'
                sh 'whoami'
                sh 'node --version'
            }
        }
    }
}
