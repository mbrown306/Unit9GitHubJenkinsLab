node {
  agent any

  tools {
    maven "maven3"
  }

  stages{
     stage('checkout sources') {
           // You should change this to be the appropriate thing
           git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
     }
     stage('Build') {
       steps {
          echo "test"
        }
     }
  // you should add a test report here
  }
}
