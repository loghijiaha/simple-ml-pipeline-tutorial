pipeline {
    agent {
        docker { image 'frolvlad/alpine-glibc:alpine-3.12' }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo "hi"' 
            }
        }
    }
}
