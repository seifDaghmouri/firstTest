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
                sh 'sudo service postgresql restart'
                
                echo 'success'
               
            }
        }
        stage('BD restart') {
            steps {
                sh 'service odoo-server restart'
                echo 'success'

            }
        }
    }
}
//}