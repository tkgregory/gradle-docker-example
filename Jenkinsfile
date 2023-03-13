pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo 'This is uday'
            }
        }
        stage('Build1'){
            steps {
              sh './gradlew build'
            }
            
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
    }
}
