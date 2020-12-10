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
                        sh '''npm install pm2@latest -g'''
                        sh '''pm2 start app.js '''
                        sh '''pm2 log '''
                    }
                }
        
    }
}

