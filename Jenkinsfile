pipeline {
    agent {
        docker { 
                image 'frolvlad/alpine-miniconda3' 
                args 'pip installl numpy'
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
