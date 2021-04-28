pipeline {
    agent any 
    stages {
        /*stage('Git checkout') {
            steps {
               checkout scm
            }*/
            
        stage('BD restart') {
            steps {
                //def cmd ="sudo service odoo-server restart"
                sh 'sudo service postgresql restart'
                
                echo 'success'
               
            }
        }
        stage('Odoo restart') {
            steps {
                sh 'service odoo-server restart'
                echo 'success'

            }
        }
    }
}
//}