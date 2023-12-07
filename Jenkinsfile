pipeline {
    agent none
    stages {
        stage ('Check maven version'){
            agent {
                docker 'maven:3-alpine'
            }
            steps {
                echo "maven version"
                sh "mvn --version"
            }
        }
        stage ('Check java version'){
            agent {
                docker 'openjdk:8-jre'
            }
            steps {
                echo "java version"
                sh "java -version"
            }
        }
    }
}
