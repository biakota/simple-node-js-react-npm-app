pipeline {
    agent {
        docker {
            image 'node' 
            args '-p 3000:3000' 
        }
    }
    environment { 
    HTTP_PROXY = 'http://10.225.3.1:3128'
   }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
