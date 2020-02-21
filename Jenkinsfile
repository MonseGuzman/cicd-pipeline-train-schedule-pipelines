pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh './gradlew build --no-daemon'
                sh 'echo "artifact file" > dist/trainSchedule.zip'
            }
        }
    }
    post {
        always {
            archiveArtifacts artifacts: 'dist/trainSchedule.zip', onlyIfSuccessful: true
        }
    }
}