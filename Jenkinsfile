pipeline {
    agent any
    stages {
        stage ('BUILD') {
            steps {
                echo 'Deploying additional pylons'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}