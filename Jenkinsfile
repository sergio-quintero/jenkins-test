stages {
  stage('Generate Kubernetes Manifests') {
    steps {
    sh '''
    echo "BUILD=1234" > build.properties
    '''
    }
  }
}
post {
  always {
    archiveArtifacts artifacts: 'dist/*.yaml', fingerprint: true
    archiveArtifacts artifacts: 'build.properties', fingerprint: true
  }
}
