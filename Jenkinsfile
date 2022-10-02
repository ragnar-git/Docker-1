pipeline {
    agent {
        label {
            label 'built-in'
        }
    }
    stages {
        stage ('22Q1'){
            steps{
            dir ('/mnt/docker/22Q1/'){
             sh 'rm -rf /mnt/docker/22Q1/*'
             sh 'git clone https://github.com/ragnar-git/Docker-1.git /mnt/docker/22Q1/. -b 22Q1'
             sh "cp /mnt/docker/22Q1index.html server-1:/usr/local/apache2/htdocs/"
            }
            }
        }
    }
}
