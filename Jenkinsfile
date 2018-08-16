node{ 
    def mvnHome
    stage('Preparation'){   
        cleanWs()
        checkoutscm
        mvnHome = tool 'M3'
    }
    stage('Creating Package'){
        sh "${mvnHome}/bin/mvn package"
    }
}
