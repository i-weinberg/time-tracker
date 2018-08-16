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
            junit 'build/reports/**/*.xml'
        }
    }
}
