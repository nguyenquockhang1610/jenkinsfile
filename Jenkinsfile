﻿pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh '''
                        ssh root@10.162.68.66
                        cd odoo17
                        ./down.sh
                        ./start.sh
                    '''
                }
            }
        }
    }
}
