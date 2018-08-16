node{ 
    def mvnHome
    stage('Preparation'){
        cleanWs()      
        mvnHome = tool 'm3'
    }
    stage('Creating Package'){
        sh "{mvHome}/bin/mvn package"
    }
}
