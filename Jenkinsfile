pipeline {
    agent any

    stages {
       stage('Build') {
            steps {
               git branch: 'main', credentialsId: 'ml_pipeline', url: 'https://github.com/AthaulRai/ml_pipeline.git'
            }
        }
    }
}
