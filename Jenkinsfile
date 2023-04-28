pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World' > build.properties
                archiveArtifacts 'build.properties'
            }
        }
    }
}
