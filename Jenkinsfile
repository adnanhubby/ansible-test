peline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                git "https://github.com/adnanhubby/ansible-test.git"
                
            }
        }
        stage(" execute Ansible") {
           steps {
                ansiblePlaybook credentialsId: 'asajid-aws.pem', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'dev.inv', playbook: 'aws.yaml'
            }    
        }    
    }
}
