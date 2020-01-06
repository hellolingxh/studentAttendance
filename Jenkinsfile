pipeline {
    agent any

    stages {
        stage ('Compile') {
            steps {
                withMaven(maven: 'MAVEN3.6.3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Test') {
                    steps {
                        withMaven(maven: 'MAVEN3.6.3') {
                            sh 'mvn test'
                        }
                    }
                }
    }
}