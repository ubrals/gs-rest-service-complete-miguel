pipeline {
    agent { 
        docker { 
//            image 'maven:3.3.3' 
//            image 'maven:3.5.4' 
//            image 'maven:3-alpine' 
            image 'jenkinsci/blueocean' 
//            args '-v /home/ec2-user/.m2' 
        } 
    }
    stages {
        stage('build') {
            steps {
//                sh 'mvn --version'
                sh 'mvn -B package'
            }
        }
        stage('test') {
            steps {
                sh 'mvn -B test'
            }
        }
    }
}

