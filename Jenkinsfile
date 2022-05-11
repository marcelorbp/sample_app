#!/usr/bin/env groovy
pipeline {
  agent { any { image 'node:12.16.2' args '-p 3000:3000' } }
    tools {
        nodejs "NODE"
    }

    stages{
       
        stage('Build') {
            steps {
                sh 'npm --production=false install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running Tests!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy somewhere!'
            }
        }
    }
}

