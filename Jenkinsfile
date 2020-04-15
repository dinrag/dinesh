pipeline {
    agent any

    stages {
        stage('---clean--') {
            steps {
                sh "mvn clean"
            }
        }
        stage('---test----') {
            def mvnHome= tool name: 'maven'
   
            sh "${mvnHome}/bin/mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
