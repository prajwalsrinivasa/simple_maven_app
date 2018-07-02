pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /home:/home' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
