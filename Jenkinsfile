pipeline {
    agent any 
    stages {
        /*stage('Git checkout') {
            steps {
               checkout scm
            }*/
            
        stage('Odoo cmd') {
            steps {
                //def cmd ="sudo service odoo-server restart"
                // sh 'service odoo-server restart'
                echo 'success'
                sh 'service postgresql restart'
                echo 'success'
               
                
            }
        }
    }
}
//}