pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
     stage('Checkout') {
            steps {
                echo 'Checkout the code...'
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/devopscloudworld/demo.git']])
            }
        }
        
    }
}
