pipeline{
    agent any
    
    stages {
        stage('Cleaning Stage'){
            steps{
                sh 'mvn clean'
            }
        }
        stage('Intalling Stage'){
            steps{
                sh 'mvn install'
            }

        }
        stage('Testing Stage'){
            steps{
                sh 'mvn test'
            }
        }
    }
}