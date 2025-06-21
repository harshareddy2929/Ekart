pipeline {
    agent any

        }

    stages {
        stage('Clone Repository') {
            steps {
                git credentialsId: 'git-credentials', url: 'https://github.com/harshareddy2929/Ekart.git'
                branch: 'feature'
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
