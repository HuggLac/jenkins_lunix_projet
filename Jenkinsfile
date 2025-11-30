pipeline {
    agent any
    environment {
        PYTHON_HOME = '/usr/bin/'
        PATH = "${env.PATH};${PYTHON_HOME}"
    }
  
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/HuggLac/jenkins_lunix_projet.git'
            }
        }
        stage('Build') {
            steps {
                script {
					sh 'echo "Running on Windows"'
					sh 'python helloworld.py'					
                }
            }
        }
    }
}
