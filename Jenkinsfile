node {

     stage('checkout sources') {
           // You should change this to be the appropriate thing
           git url: 'https://github.com/mbrown306/Unit9GitHubJenkinsLab'
     }
     stage('Build') {
     withMaven( maven: 'maven3') {
        sh 'mvn -version'
        echo "test"
    }
     }
     stage('Test') {
     withMaven( maven: 'maven3') {
        sh 'mvn test' 
    }
     }
}
