Pipeline {
    agent any

    stages {
        stage('Checkout Sources') {
            steps {
                echo 'Building..'
               git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
