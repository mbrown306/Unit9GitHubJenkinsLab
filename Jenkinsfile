node {

     stage('checkout sources') {
           // You should change this to be the appropriate thing
           git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
     }
     stage('Build') {
     withMaven( maven: 'maven3') {
        sh 'mvn package'
        echo "test"
    }
  }
     stage('Test') {
     withMaven( maven: 'maven3') {
        sh 'mvn test'
    }
  }
     stage('Deploy'){
       echo 'test'
     }
 }

  post {
    always {
      junit 'target/surefire-reports/TEST-*.xml'
    }
 }
