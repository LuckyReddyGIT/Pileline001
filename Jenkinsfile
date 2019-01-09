pipeline {
    agent any 
    stages {
        stage('Clone repo and clean it') {
            steps {
                sh "git clone https://github.com/LuckyReddyGIT/Pileline.git"
                sh "mvn clean -f Pileline"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test -f Pileline"
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package -f Pileline"
            }
        }
    }
}
