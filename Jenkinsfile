pipeline {
    agent any 
    stages {
        stage('Git checkout') {
            
                checkout scm
            
            
        stage('Odoo cmd') {
            steps {
                def cmd ="sudo service odoo-server restart"
                sh '$cmd'
                echo 'success'
            }
        }
    }
}
}