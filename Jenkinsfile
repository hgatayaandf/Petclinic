pipeline {
    agent any
    
    tools {
        jdk 'jdk'
        maven 'maven'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/hgatayaandf/Petclinic.git'
            }
        }

        stage('Maven Compile done') {
            steps {
                sh "mvn clean compile"
            }
        }
    }
}
