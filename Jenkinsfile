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
                 mail to: 'venkaiahkuncham123@gmail.com',
                 subject: "Success: Job '${env.JOB_NAME}' [Build #${env.BUILD_NUMBER}]",
                 body: "The build completed successfully. View details here: ${env.BUILD_URL}"
        }
    }
}
