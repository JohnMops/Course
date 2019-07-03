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
                script{
                   sh label: '', script: '''git checkout Lidor
		   echo Lidor Abo > lidorabo.txt
		   git add .
                   git commit -m "pushing to git"
                   git push origin Lidor
                   '''
			
                }
            }
        }
    }
}
