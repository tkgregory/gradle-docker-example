pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                sh './gradlew assemble'
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
