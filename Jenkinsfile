pipeline {
    agent {
        docker {
            image 'alpine:3.7' 
        }
    }
    
    stages {
        stage('Build') { 
            steps {
                step([$class: 'IPythonBuilder', parserType: 'file', filePath: "train_model.ipynb"])
            }
        }
        stage('Predict') { 
            steps {
                step([$class: 'IPythonBuilder', parserType: 'file', filePath: "predict_model.ipynb"])
            }
        }
        
    }
}
