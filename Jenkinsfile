pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh './gradlew build --no-deamon'
                archiveArtifacts artifacts: '/dist/trainSchedule.zip'
            }
    }
}
