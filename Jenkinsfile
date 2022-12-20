pipeline{
    agent any
    
    stages {
        stage('Cleaning'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    bat 'mvn clean'
                }
            }
        }
        stage('Installing'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    bat 'mvn install'
                }
            }
        }
        stage('Testing'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    bat 'mvn test'
                }
            }
        }
    }
}