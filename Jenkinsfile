pipeline {
    agent any
    stages {
        stage("SonarQube") {
            steps {
                sh '''
                    sonar-scanner \
                          -Dsonar.projectKey=mre \
                          -Dsonar.sources=./src \
                          -Dsonar.host.url=http://localhost:9000 \
                          -Dsonar.login=sqp_0ab21867a70cf835dbbddcc3ca63ce6bf287ffd0
                '''
            }
        }
    }
}
