pipeline {
    // agent any

    agent {
        docker { image 'maven:3.6.3' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
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
    
    // cleanup
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
