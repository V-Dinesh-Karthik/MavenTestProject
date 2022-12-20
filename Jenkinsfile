pipeline{
    agent any
    
    stages {
        stage('Cleaning'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn clean'
                }
            }
        }
        stage('Installing'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn install'
                }
            }
        }
        stage('Testing'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn test'
                }
            }
        }
    }
}