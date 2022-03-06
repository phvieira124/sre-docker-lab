pipeline {
    agent {
        label "master"
    }

    stages {
        stage('checkout:git') {
            steps {
                 git credentialsId: '15983b9a-5411-410b-bed1-3bb1c7ecdb34', url: 'https://github.com/phvieira124/sre-docker-lab.git'
            }
        }

        stage('test:mvn') {
            steps {
                sh 'mvn test -f ./hr-eureka-server'
                sh 'mvn test -f ./hr-payroll'
                sh 'mvn test -f ./hr-worker'
                sh 'mvn test -f ./netflix-zuul-api-gateway-server'
            }
        }

        stage('code_analise:sonar') {
            steps {
                 h 'mvn sonar:sonar -f ./hr-eureka-server'
                sh 'mvn sonar:sonar -f ./hr-payroll'
                sh 'mvn sonar:sonar -f ./hr-worker'
                sh 'mvn sonar:sonar -f ./netflix-zuul-api-gateway-server'
            }
        }

    }
}


