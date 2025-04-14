pipeline {
    agent any

    tools {
        nodejs 'nodejs23' // Utilisation de Node.js configuré dans Jenkins
    }

    environment {
        NODE_ENV = 'test'
      
    }

    stages {

       

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test' // nécessaire pour sonar si tu veux le coverage
            }
        }

       

     

        stage('Deploy') {
            steps {
                sh 'echo DEEPPPLLOOYY'
            }
        }
    }
}
