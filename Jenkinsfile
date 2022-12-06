pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                git "https://github.com/adnanhubby/ansible-test.git"
                cd 'ansible-playbook aws.yaml'
            }  
        }
    }
}
