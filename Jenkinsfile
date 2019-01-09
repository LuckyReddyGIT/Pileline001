pipeline {
    agent any 
    stages {
        stage('Clone repo and clean it') {
            steps {
                sh "git clone https://github.com/LuckyReddyGIT/Pileline001.git"
                sh "mvn clean -f Pileline001"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test -f Pileline001"
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package -f Pileline001"
            }
        }
    }
}
