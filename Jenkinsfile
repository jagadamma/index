pipeline {
    agent any
    stages {
       stage ('nginx installation s1') {
          steps {
            sh 'sudo yum install nginx -y'
            sh 'sudo service nginx start'
            }
        }
      stage ('copying the path s1') {
            steps {
                sh 'sudo cp -r /var/lib/jenkins/workspace/j1/index.html /usr/share/nginx/html/'
                sh 'sudo service nginx restart'
            }
        }
    }
}
      
