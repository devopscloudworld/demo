pipeline {
    agent any

    stages {
        stage('Checkout my code') {
            steps {
                echo 'Checkout git hub code...'
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/devopscloudworld/demo.git']])
            }
        }
        
         stage('Build code') {
            steps {
                echo 'Building...'
            }
        }
        
        stage('Upload') {
            steps {
                echo 'UPloading.......'
            }
        }
        
        
    }
}
