pipeline {
    agent{label 'master'}
    tools {maven "M3"}

    stages {
        stage('Checkout') {
            steps{
                git branch: 'main', url: 'https://github.com/Llelepipede/JenkinsTest'
            }
        }
        stage('Build') {
            steps{
                bat 'mvn compile'
            }
        }
    }
}
