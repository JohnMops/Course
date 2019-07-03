def ls_command
pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('checkout'){
            steps {
                script {
                    git credentialsId: 'devopint', url: 'https://github.com/DevOpsINT/Course.git'
                }
            }
        }
        stage('shell command example') {
            steps {
                script {
                   sh label: '', script: 'echo Hello World > lidor.txt'
		   sh label: '', script: 'cat lidor.txt'
                }
            }
        }
    }
}
