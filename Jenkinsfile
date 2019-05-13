pipeline {
    agent any

    stages{

        stage('Checkout SVM'){
            git branch: 'master' , url:'https://github.com/LeticiaEulalia/endCareer.git'
        }
        
        stage('Install node modules'){
            steps {
                sh "npm install"
            }
        }

        stage('Build'){
            sh "npm run build:ssr"
        }
    }
}
