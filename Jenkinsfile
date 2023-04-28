pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World' > build.properties
            }
        }
    }
}
post {
  always {
    archiveArtifacts artifacts: 'dist/*.yaml', fingerprint: true
    archiveArtifacts artifacts: 'build.properties', fingerprint: true
  }
}
