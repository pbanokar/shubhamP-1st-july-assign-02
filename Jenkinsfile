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
                sh "cp -r dev.html /var/www/html/
                sh "chmod -R 777 /var/www/html/dev.html"
            }
        }
        }
}
