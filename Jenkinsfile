pipeline {
    agent {
        docker { 
                image 'frolvlad/alpine-miniconda3' 
               }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'pip install numpy' 
            }
        }
    }
}
