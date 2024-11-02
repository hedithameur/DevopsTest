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
		stage('Scan'){
			steps {
				withSonarQubeEnv(installationName: 'station-ski-project'){
					sh './mvnw clean sonar:sonar'
				}
			}
		}
    }
}
