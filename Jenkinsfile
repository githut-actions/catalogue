pipeline {
    agent {
        label 'AGENT-1'
    }
    environment {
        appVersion = ''
    }
    stages {
        stage('Read package.json') {
            steps {
                script {
                    def packageJson = readJSON file: 'package.json'
                    appVersion = packageJson.version
                    echo "Application Version: ${appVersion}"
                
                
                }
            
            
            
            }
        
        
        
        }
        stage ('Install Dependies')
            steps {
                script {
                    sh """
                     npm install 
                     
                     """
                
                }
            
            
            }
    
    
    
    }



}