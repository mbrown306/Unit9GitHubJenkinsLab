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
           echo "test"
          }
     }
     stage('Deploy') {
           withMaven( maven: 'maven3') {
           echo "test"
           sh 'mvn deploy'
       }
     }
 }
