pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Testing maven') {
            steps {
                sh 'mvn -version'
          
            }
        }
        stage('Checkout GIT') {
            steps {
                echo 'Pulling...';
                git branch: 'main',
                    url: 'https://github.com/hedithameur/DevopsTest.git'
            }
        }
    
    }
    

}