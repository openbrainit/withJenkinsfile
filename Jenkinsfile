pipeline {
    agent { docker { image 'maven:3.3.3' } }
    environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE    = 'sqlite'
    }
    stages {
        stage('build') {
            steps {
                echo "${DB_ENGINE}"
                sh 'mvn --version'
                sh 'touch test'
            }
        }
    }
}