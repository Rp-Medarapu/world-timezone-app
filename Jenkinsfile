pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat 'mvn clean install'
            }
        }
        stage('deploy') {
            steps {
                bat 'mvn package deploy -DmuleDeploy'
            }
        }
    }
}