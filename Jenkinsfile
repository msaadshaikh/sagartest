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
  
  stage('Quay stage') {
          steps {
       
            script {
            echo 'Cxone stage.'
            quay()
        }
      
    }
  }
  stage('Service Now') {
          steps {
       
            script {
            echo 'Service Now stage starting.'
          //  serviceNowTicketStatus()
        }
      
    }
  }
   stage('Deploy') {
        steps {
       
          script {
           
            deployApp()
            echo 'Build completed using shared library function.'
        }
      
    }
}



       
    }
}
