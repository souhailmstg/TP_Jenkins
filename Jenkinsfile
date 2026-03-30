pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo 'Cloning repository...'
                git 'https://github.com/souhailmstg/TP_Jenkins.git'
            }
        }

        stage('Compile Java Files') {
            steps {
                echo 'Compiling Java files...'
                bat 'javac *.java'
            }
        }

        stage('Run Program') {
            steps {
                echo 'Running HelloWorld...'
                sh 'java HelloWorld'
            }
        }

    }
}
