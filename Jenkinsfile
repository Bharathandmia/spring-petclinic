pipeline {
    agent { label 'first' }
    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/Bharathandmia/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
