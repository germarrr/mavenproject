pipeline {
    agent any
	tools {
		maven 'maven_3_6_1'
	}
    stages {
	    stage('Initialize Stage') {
            steps {
				echo 'INITIALIZE Stage...'
				echo 'MAVEN_HOME = ${MAVEN_HOME}'
				sh 'mvn clean'
            }
        }
        stage('Build Stage') {
            steps {
				echo 'BUILD Stage...'
				sh 'mvn validate'
				sh 'mvn compile'
				sh 'mvn test'
				sh 'mvn package'
            }
        }
        stage('Testing Stage') {
            steps {
				echo 'TESTING Stage...'
            }
        }
    }
}
