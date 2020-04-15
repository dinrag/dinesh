pipeline {
    agent any

    stages {
        stage ('compile') {
            steps {
                withMaven(maven : 'apache-maven-3.6.3') {
                    sh 'mvn clean complile'
                }
            }
        }
    }
}
