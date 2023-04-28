pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                    sh '''
                        echo "BUILD=1234" > build.properties
                        '''
                archiveArtifacts 'build.properties'
            }
        }
    }
}
