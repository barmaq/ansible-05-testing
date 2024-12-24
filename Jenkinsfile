pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Sync Git') {
            steps {
                dir('/home/jenkins/test') {
                    git(url: 'https://github.com/barmaq/ansible-05-testing', branch: 'main')
                }
            }
        }
        stage('Run molecule') {
            steps {
                dir('/home/jenkins/test') {
                    sh 'python3 -m venv venv && . venv/bin/activate && pip3 install ansible molecule molecule_docker future molecule_podman && molecule test -s default && deactivate'
                }
            }
        }
    }
}
