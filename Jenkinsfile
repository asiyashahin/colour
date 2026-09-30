pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                dir('flutter_app') {
                    bat 'flutter pub get'
                }
            }
        }

        stage('Test') {
            steps {
                dir('flutter_app') {
                    bat 'flutter test'
                }
            }
        }
    }
}