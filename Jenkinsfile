 pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/kunal015-P/pythonhelloworld.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    dockerImage = docker.build('python-hello-world')
                    echo 'Docker Image build suceesfull'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    dockerImage.run()
                    echo 'Container created'
                }
            }
        }
       stage('Stage updated by Kunal') {
            steps {
                script {
                    echo 'Updated by kunal'
                }
            }
        }
      stage('Stage updated by Mithare') {
            steps {
                script {
                    echo 'Updated by Mithare'
                
            }
        }
    } 
                   
    }
}
