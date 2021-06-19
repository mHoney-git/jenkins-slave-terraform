pipeline {
    agent any 
    stages {
        stage ('installing jenkins on jenkins-slave-terraform instance') {
            steps {
                ansiblePlaybook credentialsId: 'AWS-SSH-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'site.yml'
              }
        }
    }
}