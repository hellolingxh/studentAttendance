pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "Maven3.6.3"
    }

    stages {
        stage ('Compile') {
            steps {
               sh 'mvn clean compile'
            }
        }

        stage ('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}