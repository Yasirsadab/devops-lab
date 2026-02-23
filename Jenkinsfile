pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Yasirsadab/devops-lab.git',
                    credentialsId: 'github-token'
            }
        }

        stage('Build') {
            steps {
                sh 'javac hello.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java hello'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the job'
            }
        }
    }
}
