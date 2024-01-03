pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Sử dụng sh để thực hiện các lệnh trên một máy từ xa thông qua SSH
                    sh '''
                        ssh root@10.162.68.66 'cd odoo17 && ./down.sh && ./start.sh'
                    '''
                }
            }
        }
    }
}
