node {
     stage('checkout sources') {
           // You should change this to be the appropriate thing
           git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
     }
     stage('Build') {
        steps {
            withMaven( maven: 'maven3') {
           sh 'mvn package'
           echo "test"
         }
       }
     }
     stage('Test') {
        steps {
           withMaven( maven: 'maven3') {
           sh 'mvn test'
           echo "test"
          }
       }
     }
     stage('Deploy') {
        steps {
           withMaven( maven: 'maven3') {
           echo "test"
          }
       }
     }
 }
