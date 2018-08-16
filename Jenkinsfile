node{ 
    def mvnHome
    stage('Preparation'){
        cleanWs()      
        mvnHome = tool 'M3'
    }
    stage('Creating Package'){
        sh "{mvHome}/bin/mvn package"
    }
}
