pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                sh 'echo "Welcome to the Docker Agent Tutorial"'
                sh 'pip install -r requirements.txt'
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
