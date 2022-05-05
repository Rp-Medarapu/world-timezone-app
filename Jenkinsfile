pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            	withMaven(maven:'maven'){
                	bat 'mvn -f world-demo-api/pom.xml clean install'
                }
            }
        }
        stage('deploy') {
            steps {
            	withMaven(maven:'maven'){
                	bat 'mvn -f world-demo-api/pom.xml package deploy -DmuleDeploy'
                }
            }
        }
    }
}