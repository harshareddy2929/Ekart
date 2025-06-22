pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                url: 'https://github.com/harshareddy2929/Ekart.git'
                            }
                
            }
        stage('Build') {
            steps {
                echo 'Building Java application with Maven...'
                sh 'mvn clean package'
            }
        }
        }
                  
      post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
