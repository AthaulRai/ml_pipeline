pipeline {
    agent any

    stages {
      stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'd788a3ee-b5b8-4b58-8f4e-9d8074a2e0a1', url: 'https://github.com/AthaulRai/ml_pipeline.git']]])
            }
        }
       stage('Build') {
            steps {
               git branch: 'main', credentialsId: 'ml_pipeline', url: 'https://github.com/AthaulRai/ml_pipeline.git'
            }
        }
    }
}


