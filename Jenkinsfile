pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
    }
}