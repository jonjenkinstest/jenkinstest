@Library("jenkins-shared-libs@master") _

pipeline {
    agent any
    environment {
        JONS_SECRET     = credentials('jons-secret')
    }
    stages {
        stage('One') {
            steps {
                echo "My secret: ${JONS_SECRET}"
            }
        }
        stage('Two') {
            steps {
                build('test param')
            }
        }
    }
}
