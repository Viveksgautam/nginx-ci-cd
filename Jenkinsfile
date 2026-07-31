pipeline{
    agent any 

    stages {
        stage('Deploy code') {
            steps {
                sh '''
                git clone 'https://github.com/Viveksgautam/nginx-ci-cd.git'
                cd nginx-ci-cd
                sudo cp -r * /var/www/html/
                sudo systemctl restart nginx
                '''
            }
        }
    }
}
