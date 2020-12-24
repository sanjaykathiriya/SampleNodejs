pipeline {
   agent any
  
    
    stages {
        stage('Build') {
            steps {
                 '''npm install'''
            }
        }
        stage('Test') {
            steps {
                '''npm run build'''
            }
        }
        stage('deploy') {
                    steps {
                         '''npm install -g serve'''
                           '''serve -s build '''
                     
                       
                        
                        
                    }
                }
        
    }
}

