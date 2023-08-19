pipeline {
    agent { label 'JDK'}
    stages { 
        stage ('GIT') {
            steps {
                git url: 'https://github.com/spring-projects/spring-petclinic.git'
                    branch: 'main'
                    
            }
        }
        stage ('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}