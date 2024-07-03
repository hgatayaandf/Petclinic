pipeline {
    agent any
    
    tools {
        jdk 'JDK'
        maven 'maven'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/hgatayaandf/Petclinic.git'
            }
        }

        stage('Maven Compile') {
            steps {
                sh "mvn clean compile"
            }
        }
    }
}
