pipeline {
    agent any

    stages {

        stage('CHECKOUT stage') {
          steps {
       
            script {
            echo 'this is checkout stage.'
        }
      
      }
    }
  
  stage('CxOne CHECKMARX stage SAST SCA') {
          steps {
       
            script {
            echo 'Cxone stage.'
            cxOneSastSca()
        }
      
    }
  }
   stage('SONARQUBE stage') {
          steps {
       
            script {
            echo 'Cxone stage.'
            //sonarQubeScan()
        }
      
    }
  }
       

       stage('Build') {
        steps {
       
          script {
           
            buildApp()
            echo 'Build completed using shared library function.'
        }
      
    }
}

 stage('Deploy') {
        steps {
       
          script {
           
            deployApp()
            echo 'Deply completed using shared library function.'
        }
      
    }
}


       
    }
}
