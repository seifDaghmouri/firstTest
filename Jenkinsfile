pipeline {
    agent any 
    stages {
        steps{
        /*stage('Git checkout') {
            steps {
               checkout scm
            }*/

        stage('BD restart') {
            steps {
                //def cmd ="sudo service odoo-server restart"
                sh 'service postgresql restart'
                echo 'success'
            }

        stage('Odoo restart') {
            steps {
                //def cmd ="sudo service odoo-server restart"
                sh 'service odoo-server restart'
                echo 'success'
            }
        }
    }
}
}
}