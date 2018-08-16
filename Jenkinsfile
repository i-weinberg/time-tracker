node{ 
    def mvnHome
    stage('Preparation'){   
        cleanWs()
        checkout scm
        mvnHome = tool 'M3'
    }
    stage('Creating Package'){
        sh "${mvnHome}/bin/mvn package"
    }
    post {
        always {
            archiveArtifacts artifacts: 'build/libs/**/*.jar', fingerprint: true
            junit 'build/reports/**/*.xml'
        }
    }
}
