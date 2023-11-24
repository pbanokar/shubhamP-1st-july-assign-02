pipeline {
    agent {
        label {
            label "built-in"
            customWorkspace "/mnt/test1"
        }
    }
    stages {
        stage ("one") {
            steps {
                sh "yum install httpd -y"
                sh "systemctl start httpd"
                sh "echo 'hello' >> /var/www/html/index.html"
                sh "chmod -R 777 /var/www/html/index.html"
            }
        }
        }
}
