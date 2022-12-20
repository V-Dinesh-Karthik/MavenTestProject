pipeline{
    agent any
    
    stages {
        stage('Cleaning Stage'){
            withMaven(maven: "MAVEN_HOME"){
                sh 'mvn clean'
            }
        }
        stage('Intalling Stage'){
            withMaven(maven: "MAVEN_HOME"){
                sh 'mvn install'
            }
        }
        stage('Testing Stage'){
            withMaven(maven: "MAVEN_HOME"){
                sh 'mvn test'
            }
        }
    }
}