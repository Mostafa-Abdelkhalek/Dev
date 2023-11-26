pipeline {
    agent any 
    
    tools {
        NodeJS 'nodejs'
    }
    stages {
        stage ('checkout ') {
            steps {
                checkout scm 

            }
        }
        stage ('install dependinces') {
            sh 'npm install'

        }
        stage ('Build') {
            sh 'npm run build'

        }
        stage ('test') {
            sh 'npm test'
        }
    }   
}