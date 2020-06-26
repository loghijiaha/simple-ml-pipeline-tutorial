pipeline {
    agent any
    
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
