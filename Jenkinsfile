pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                sh "chmod u+x gradlew"
                sh "./gradlew compileJava"
            }
        }
        stage ('Unit test') {
            steps {
                sh "./gradlew test"
            }
        }
    }
}