pipeline {
    agent {
        label "SAO-DXM1VW2"
    }

    stages {
        stage('git') {
            steps {
                 git credentialsId: 'd7a59324-293f-4ddd-9a10-997228c1ee72', url: 'https://github.com/phvieira124/sre-docker-lab.git'
            }
        }

        stage('build') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
