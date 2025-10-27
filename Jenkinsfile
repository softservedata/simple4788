pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Compile') {
            steps {
                bat 'mvn -B compile'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn -B package -DskipTests'
            }
        }

        stage('Unit Test') {
            steps {
                bat 'mvn -B test'
            }
        }

        stage('done') {
            steps {
                echo 'finish'
            }
        }
    }
}
