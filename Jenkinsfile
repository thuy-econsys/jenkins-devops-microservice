pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build stage'
            }
        }
		stage('Test') {
            steps {
                echo 'Test stage'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'Integration Test stage'
            }
        }
    } 
    
    post {
        always {
            echo 'Always posts'
        }
        success {
            echo 'Post is successful'
        }
        failure {
            echo 'Post failed'
        }
    }
}
