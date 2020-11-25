
node {

  stage('checkout sources') {
        // You should change this to be the appropriate thing
        git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
  }
  stage('Build') {
    steps {
       ssh "mvn -version"
       sh  'mvn clean package'
     }
  }
  stage('Test') {
    // you should build this repo with a maven build step here
    echo "hello"
  }

  // you should add a test report here
}
