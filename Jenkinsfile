pipeline {
    agent any
    tools {nodejs "mynodejs"}
    stages {
        stage('Hello') {
            steps {
                git 'https://github.com/SANA-TASMIA/aws_codebuild_codedeploy_nodeJs_demo.git'
                echo 'v3 changes declarative'
                sh 'cat index.js'
                
            }
        }
        stage('build') {
            steps {
                sh 'npm install'
                
            }
        }
    }
}