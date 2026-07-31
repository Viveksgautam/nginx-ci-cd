pipeline{
    agent any 

    stages {
        stage('Deploy code') {
            steps {
                sh '''
                rm -r nginx-ci-cd
                git clone 'https://github.com/Viveksgautam/nginx-ci-cd.git'
                cd nginx-ci-cd
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
