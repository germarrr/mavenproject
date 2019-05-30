pipeline {
    agent any
	tools {
		maven 'maven_3_6_1'
	}
    stages {
	    stage('Initialize Stage') {
            steps {
				echo 'Initialize Stage...'
            }
        }
        stage('Compile Stage') {
            steps {
				echo 'Compile Stage...'
				sh 'mvn clean compile'
            }
        }
        stage('Testing Stage') {
            steps {
				echo 'Testing Stage...'
				sh 'mvn test'
            }
        }
    }
}
