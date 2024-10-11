pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/yourusername/my-jenkins-ansible-project.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook ansible/playbook.yml -i ansible/inventory'
            }
        }
    }
}
