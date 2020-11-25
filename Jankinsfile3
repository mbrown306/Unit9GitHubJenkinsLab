node {
    agent any

    stages {
        def mavHome= tool 'Maven3'
        stage('Checkout') {
            steps {
                echo 'Building..'
                 checkout([$class: 'GitSCM', branches: [[name: 'dev9']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '3a286bc5-00c1-458c-ba6c-7b27ed5a95a4', url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab']]])
            }
        }
        stage('Build') {
            steps {
                withMaven(maven : 'Maven3') {
                    sh 'mvn clean compile'
               }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven : 'Maven3') {
                    sh 'mvn test' 
               }
               post {
                   always {
                       junit 'target/*.xml'
                   }
            }
        }
        stage('Deploy') {
            steps {
                withMaven(maven : 'Maven3') {
                    sh 'mvn deploy'
               }
           }
        }
    }
}
