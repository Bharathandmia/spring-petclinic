pipeline {
    agent { label 'first'}
    stages {
        stage('scm') {
            steps {
                git 'https://github.com/Bharathandmia/spring-petclinic.git'
            }
        }
        stage('build') {
            steps {
                sh script: 'mvn clean package'
            }
        }
     }
}
