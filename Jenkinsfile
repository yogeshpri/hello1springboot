@Library('my-shared-lib@main') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yogeshpri/hello1springboot.git'
            }
        }

        stage('Build with Maven') {
            steps {
                mavenBuild()
            }
        }
    }
}

