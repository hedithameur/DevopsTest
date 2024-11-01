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
    }
}
