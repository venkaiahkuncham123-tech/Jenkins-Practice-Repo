pipeline {
    agent any

    stages {
        stage('Job 1'){
            steps {
                sh 'echo job1'
            }
        }
        stage('Job 2'){
            steps {
                sh 'echo job2'
            }
        }
    }
    post {
        success {
            build job: 'Free Style Job'
        }
    }
}
