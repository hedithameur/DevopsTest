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
		stage('GIT') {
		steps {
			echo 'Getting Project from Git'
			url : 'https://github.com/hedithameur/DevopsTest.git'
		}
		}
    
    }
}
