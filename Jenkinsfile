pipeline {
    agent {
        docker { 
                image 'frolvlad/alpine-miniconda3' 
                args 'python -c 'print("Hello World")''
               }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo "hi"' 
            }
        }
    }
}
