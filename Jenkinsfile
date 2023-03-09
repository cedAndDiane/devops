pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/cedAndDiane/devops.git"
            }
        }
        stage('build') { 
            steps {
                sh "cd devops/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd devops/ && java Main"
            }
        }
    }
 }
