node{ 
    def mvnHome
    stage('Preparation'){   
        mvnHome = tool 'M3'
    }
    stage('Creating Package'){
        sh "${mvnHome}/bin/mvn package"
    }
}
