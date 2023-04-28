pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                    sh '''
                        npm install
                        npm run import
                        npm run build
                        echo "BUILD=1234" > build.properties
                        '''
                archiveArtifacts 'build.properties'
            }
        }
    }
}
