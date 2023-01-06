pipeline {
    agent any

    stages {
        stage('validate code') {
            steps {
                echo 'Validating Code..'
                sh "/usr/share/maven/bin/mvn Validate"
            }
        }
        stage('Test code') {
            steps {
                echo 'Testing code..'
                sh "/usr/share/maven/bin/mvn Test"
            }
        }
        stage('Build') {
            steps {
                echo 'Building code....'
                sh "/usr/share/maven/bin/mvn package"
            }
        }
    }
}
