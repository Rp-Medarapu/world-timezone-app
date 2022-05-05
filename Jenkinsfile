pipeline
{
	agent any
	stages{
	stage('Build World Time Zone'){
	steps{
	bat 'mvn clean install'
	}
	}
	stage('Deploy World Time Zone'){
	steps{
	bat 'mvn package deploy -DmuleDeploy'
	}
	}
	}
}