pipline {
    agent { label 'JDK-17-MVN-3.6' }
    stages {
        stage('vcs') {
            steps {
                git clone: 'git clone https://github.com/Sysnove/flask-hello-world.git',
                branch: 'master'
            }
        }
        stage('image build') {
            sh 'docker image build -t python:3.0 .'
        }
    }
}