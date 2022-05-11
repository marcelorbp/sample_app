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
                sh 'rm -fr test_web'
                sh 'git clone https://github.com/renatasilva11/test_web.git'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'node test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy somewhere!'
            }
        }
    }
}
