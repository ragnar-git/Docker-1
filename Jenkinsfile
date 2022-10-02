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
             sh 'rm -rf /mnt/docker/22Q1/Docker-1*'
             sh 'git clone https://github.com/ragnar-git/Docker-1.git -b 22Q1'
             sh 'chmod 777 /mnt/docker/22Q1/Docker-1/index.html'
             sh "docker cp /mnt/docker/22Q1/Docker-1/index.html server-1:/usr/local/apache2/htdocs/"
            }
            }
        }
    }
}
