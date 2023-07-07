pipeline {
    agent any

    stages {
        stage('Validating') {
            steps {
                echo 'validating..'
		sh '/usr/share/maven/bin/mvn validate'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
		sh '/usr/share/maven/bin/mvn package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing....'
		sh '/usr/share/maven/bin/mvn test'
            }
        }
	stage('Message') {
            steps {
                echo 'Build is successful....'
		
            }
        }
    }
}
