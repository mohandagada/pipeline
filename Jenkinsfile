pipeline {

    agent any
	
    tools {
        maven 'MavenHome'
    }
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/mohandagada/pipeline.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
