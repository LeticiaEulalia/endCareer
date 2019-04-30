pipeline {
    agent any

    stages{

        stage('Checkout SVM'){
            git branch: 'master' , url:'https://github.com/LeticiaEulalia/endCareer.git'
        }
        
        stage('Clone repo and clean it'){
            steps {
                sh "rm -rf my-angular-app"
                sh "https://github.com/LeticiaEulalia/endCareer.git"
            }
        }

        stage('Install node modules'){
            sh "npm install"
        }
    }
}
