node {

     stage('checkout sources') {
           // You should change this to be the appropriate thing
           git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
     }
     stage('Build') {
     withMaven(jdk: 'jdk8', maven: 'maven3') {
        sh 'mvn -version'
        echo "test"
    }
     }
  // you should add a test report here
}
