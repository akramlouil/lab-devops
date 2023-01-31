pipeline {
    
    
    agent any 
    stages {
        
        
        stage ("Affichage choix "){
            steps {
                
                echo " Environnement X : $Type_Env" 
            }
        }
        
    }
    post {
        
        always {
            
            mail bcc: '', body: 'Le build N° $BUILD_NUMBER est ${currentBuild.currentResult}   voir $BUILD_URL ', cc: '', from: '', replyTo: '', subject: '[ Build N° $BUILD_NUMBER ] : ', to: 'louil.akram@gmail.com'
        }
    }
    
}
