pipeline {
    agent any
       
    stages {
         stage('Prepare') { 
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Build') { 
            steps {
                step([$class: 'IPythonBuilder', parserType: 'file', filePath: "train_model.ipynb", task:'Training', kernelName:'python'])
            }
        }
        stage('Predict') { 
            steps {
                step([$class: 'IPythonBuilder', parserType: 'file', filePath: "predict_model.ipynb", task:'Prediction', kernelName:'python'])
            }
        }
        
    }
}
