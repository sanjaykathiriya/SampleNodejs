pipeline {
   agent any
   ws("D:\cicdaws") {
  echo "awesome commands here instead of echo"
}
    
    stages {
        stage('Build') {
            steps {
                sh '''npm install'''
            }
        }
        stage('Test') {
            steps {
                sh '''npm run build'''
            }
        }
        stage('deploy') {
                    steps {
                        sh '''npm install -g serve'''
                          sh '''serve -s build '''
                     
                       
                        
                        
                    }
                }
        
    }
}

