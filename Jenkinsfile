pipeline {
    agent any
    stages('CI') {
        stage('Checkout') {
            steps {
                echo 'checkout'
                checkout scm
            }
            
        }
        stage ('build') {
            steps {
                echo 'build'
                sh 'mvn build package'
            }
            
        }
        stage ('Test') {
            steps {
                echo 'Test'
                sh 'mvn Test'
            }
            
        
        }
    }
}