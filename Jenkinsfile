pipeline {
    agent agent

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
        sucess {
            build job: 'Free Style Job'
        }
    }
}
