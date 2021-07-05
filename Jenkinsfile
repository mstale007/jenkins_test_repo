pipeline {
    agent any

    stages {
        stage('Stage 1: Execute') {
            steps {
                echo 'Starting.. Running ${BUILD_ID} on ${JENKINS_URL}'
            }
        }
        stage('Stage 2: Build') {
            steps {
                echo 'Building..'
                echo 'Python Version: \n'
                bat 'python --version'
            }
        }
        stage('Stage 3: Test') {
            steps {
                echo 'Testing..'
                echo 'Java Version: \n'
                bat 'java -version'
            }
        }
        stage('Stage 4: Release') {
            steps {
                echo 'Deploying...'
                echo 'GCC Version: \n'
                bat 'gcc --version'
            }
        }
    }
    post{
        always{
            echo "Done with everything!"
            //mail bcc: '', body: 'Yo Dawg!', cc: '', from: '', replyTo: '', subject: 'Test Mail Jenkins #01', to: 'mstale20@gmail.com'
        }
    }
}
