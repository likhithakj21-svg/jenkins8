pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                // Clone the repo (script.sh must be in this repo)
                git url: 'https://github.com/likhithakj21-svg/jenkins.git', 
                    branch: 'main'
            }
        }
        stage('Run Script') {
            steps {
                sh 'chmod +x script.sh'
                sh './script.sh'
            }
        }
    }
}
