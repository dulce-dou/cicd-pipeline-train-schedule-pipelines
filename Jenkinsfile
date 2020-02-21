pipeline {
    agent {
        dockerfile {
            filename 'dockerfile.slave'
            label 'slave'
        }
        stages {
            stage('Build') {
                steps {
                    sh './gradlew build'
                }
            }
        }
    }
}
