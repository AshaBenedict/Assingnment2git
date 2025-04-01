pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'develop',
                    credentialsId: 'your-credential-id',
                    url: 'https://github.com/your-repo.git'
            }
        }

        stage('Pull Git Content') {
            steps {
                sh 'mkdir -p /your/target/folder && cp -r * /your/target/folder/'
            }
        }
    }
}
