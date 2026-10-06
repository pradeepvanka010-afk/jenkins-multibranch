pipeline {
    agent any
    tools {
        jdk 'Jdk-17'    // Must match the name configured in Global Tools
        maven 'mvn-3.6'  // Must match the name configured in Global Tools
    }

    stages {

       stage('mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }
       stage('mvn test') {
            steps {
                sh 'mvn test'
            }
        }
       stage('mvn pkg') {
            steps {
                sh 'mvn package'
            }
        }                
    }
}
