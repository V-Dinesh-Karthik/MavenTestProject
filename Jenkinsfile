pipeline{
    agent any
    
    stages {
        stage('Cleaning Stage'){
            steps{
                withMaven(maven: "MAVEN_HOME"){
                    sh 'mvn clean'
                }
            }
        }
        stage('Intalling Stage'){
            steps{
                withMaven(maven: "MAVEN_HOME"){
                    sh 'mvn install'
                }
            }

        }
        stage('Testing Stage'){
            steps{
                withMaven(maven: "MAVEN_HOME"){
                    sh 'mvn test'
                }
            }
        }
    }
}