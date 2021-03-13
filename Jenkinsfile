pipeline {
    
    agent any
    stages {
        
        stage('build') {
            steps {
                sh 'mvn package'
                sh 'sl auth --no-diagnostic --org "467bc091-089e-48fc-a948-18c9786b1fc9" --token ""'
                sh 'sl analyze --app vulnado --java target/vulnado-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
