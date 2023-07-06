pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                //sh 'cd /home/mjetty/javasample'
                sh 'sudo cp /home/mjetty/javasample/HelloWorld.java ${WORKSPACE}'
                sh 'sudo javac HelloWorld.java'
            }
        }
        stage('Run') { 
            steps {
                sh 'java HelloWorld'
            }
        }
    }
}
