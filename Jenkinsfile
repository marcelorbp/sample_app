#!/usr/bin/env groovy
pipeline {
    agent any

    tools {
        nodejs "NODE"
    }

    stages{
       
        stage('Build') {
            steps {
                sh 'npm install'
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
