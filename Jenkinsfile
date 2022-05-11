pipeline {
    agent any

    stages {
        stage('clone repo') {
            steps {
                echo 'clone repo'
                sh 'rm -fr test_web'
                sh 'git clone https://github.com/renatasilva11/sample_app.git'
            }
        }
    
   
        stage('push repo to remote host') {
            steps {
               echo 'Hello 2'
            }
        }
       
        stage('connect') {
        steps {
          sshagent(credentials: ['webfiles']) {
           echo 'Hello 4'
      }
    }
        }
        stage('3') {
            steps {
                echo 'Hello 3'
            }
        }
    }  
  }
