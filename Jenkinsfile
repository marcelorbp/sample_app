#!/usr/bin/env groovy
pipeline {
    agent any

    tools {
        nodejs "NODE"
    }

    stages{
        stage('Checkout') {
            steps{
                echo 'clone repo'
                sh 'rm -fr sample_app'
                sh 'git clone https://github.com/renatasilva11/sample_app.git'
            }
        }
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
