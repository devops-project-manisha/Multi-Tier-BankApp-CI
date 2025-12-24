pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Building Code') {
            steps {
                sh 'mvn clean package -DskipTests'
            }
        }
    }
}
