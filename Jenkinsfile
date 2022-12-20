pipeline{
    agent any
    
    stages {
        stage(name: 'Cleaning'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn clean'
                }
            }
        }
        stage(name: 'Installing'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn install'
                }
            }
        }
        stage(name: 'Cleaning'){
            steps{
                withMaven(maven: 'MAVEN_HOME'){
                    sh 'mvn test'
                }
            }
        }
    }
}