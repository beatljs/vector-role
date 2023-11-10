pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Git checkout') {
            steps {
                // Get code from a GitHub repository
                checkout changelog: false, poll: false, scm: scmGit(branches: [[name: '**']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/beatljs/vector-role.git']])
            }
        }    
        stage('Testing role') {
            steps {
                // Run Molecule on a Unix agent.
                sh "molecule test"
            }
        }
    }
}
