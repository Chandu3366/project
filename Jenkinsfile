pipeline {
    agent any

    stages {
        stage('Validate') {
            steps {
                echo 'validating..'
		sh '/usr/share/maven/bin/mvn validate'
            }
        }
        stage('Build') {
            steps {
                echo 'Buildinggg..'
		sh '/usr/share/maven/bin/mvn package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing....'
		sh '/usr/share/maven/bin/mvn test'
            }
        }
	stage('Massage') {
            steps {
                echo 'Build is successfull....'
		
            }
        }
    }
}
