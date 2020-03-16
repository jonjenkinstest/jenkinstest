@Library("jenkins-shared-libs@master") _

pipeline {
    agent any
    stages {
        stage('One') {
            steps {
                echo 'Hi'
            }
        }
        stage('Two') {
            steps {
                build('test param')
            }
        }
    }
}
