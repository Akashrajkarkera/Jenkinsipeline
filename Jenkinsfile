pipeline {
    agent any
    parameters {
        choice(name: "environment", choices: ["DEV","ST","VAL","DEMO"], description: 'Select Environment to build and deploy')
        booleanParam(name: 'Deployment', defaultValue: true, description: 'Do you want to deploy this war file on Elasticbean environment?')
        string(name: 'TAG NAME', defaultValue: 'v2_1_', description: 'Enter the tag number with_') }

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
