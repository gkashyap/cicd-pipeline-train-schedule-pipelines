pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'cd /home/cloud_user/cicd-pipeline-train-schedule-pipelines' && './gradlew build'
		archiveArtifacts artifacts: '/dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
