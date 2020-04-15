pipeline {
    agent any

    stages {
        stage('---clean--') {
            steps {
                sh "mvn clean"
            }
        }
        stage('---test----') {
            def mvnHome= tool name: 'm3'
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
