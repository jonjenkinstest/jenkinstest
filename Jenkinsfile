@Library("jenkins-shared-libs@master") _

pipeline {
    agent any
    environment {
        JONS_SECRET     = credentials('jons-secret')
    }
    parameters {
        choice(name: 'ENVIRONMENT', choices: 'Int\nTest', description: 'Environment to deploy to')
    }
    stages {
        stage('One') {
            steps {
                echo "My secret: ${JONS_SECRET}"
            }
        }
        stage('Two') {
            steps {
                build(ENVIRONMENT)
            }
        }
    }
}
