pipeline {
    agent {
    label "test"
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
                     
                        sh '''pm2 start app.js '''
                        
                        
                    }
                }
        
    }
}

