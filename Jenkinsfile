node{ 
    def mvnHome
    stage('Preparation'){
        cleanWs()      
        mvnHome = Tool 'm3'
    }
    stage('Creating Package'){
        sh "{mvHome}/bin/mvn package"
    }
}
