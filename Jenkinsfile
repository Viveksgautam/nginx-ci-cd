pipeline{
    agent any 
    stages {
        stage('Deploy code') {
            steps {
                sh '''
                rm -r nginx-ci-cd
                git clone 'https://github.com/Viveksgautam/nginx-ci-cd.git'
                cd nginx-ci-cd
                docker build -t vivek .
                docker run -d --name vivek -p 1234:80 vivek
                '''
            }
        }
    }
}
