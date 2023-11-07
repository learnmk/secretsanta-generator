pipeline {
    agent any
    tools {
        maven "maven3"
    }

    stages {
        stage('Git scm') {
            steps {
               git 'https://github.com/jaiswaladi2468/BoardgameListingWebApp.git'
            }
        }
        stage('Clean') {
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        stage('compile') {
            steps {
                sh "mvn compile"
            }
        }
          stage('install') {
            steps {
                sh "mvn install"
            }
        }
    }
}
