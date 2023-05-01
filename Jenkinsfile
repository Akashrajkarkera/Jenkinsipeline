pipeline {
    agent any

    stages {
        stage('Fetch Jenkinsfile') {
            steps {
                git branch: 'main', url: 'https://github.com/Akashrajkarkera/Jenkinspipeline.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building the proect"'
            }
        }

        // Add more stages for testing, deploying, etc.
    }
}
