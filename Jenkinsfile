pipeline {
    agent any
    tools {
        gradle "Gradle"
    }
    stages {
        stage('code checkout') {
            steps {
              git 'https://github.com/devops1434/simple-gradle-java-app.git'
            }
        }
    stage ('gradle build') {
        steps {
            sh 'gradle clean build'
        }
    }
    stage ('gradle test') {
        steps {
            sh 'gradle test'
        }
    }
    }
}
