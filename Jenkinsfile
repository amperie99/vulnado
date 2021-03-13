pipeline {
    
    agent any
    stages {
        
        stage('build') {
            steps {
                sh 'mvn package'
                sh 'sl analyze --app vulnado --java target/vulnado-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
