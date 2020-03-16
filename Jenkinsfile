@Library("jenkins-shared-libs@master") _

pipeline {
    agent any
    stages {
        stage('One') {
            steps {
                echo 'My secret:'
                echo credentials('jons-secret')
            }
        }
        stage('Two') {
            steps {
                build('test param')
            }
        }
    }
}
