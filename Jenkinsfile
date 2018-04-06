node {
   def mvnHome = tool name: 'mvn3.5.3', type: 'maven'
   stage('Checkout') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/veersudhir83/devops-web-hackathon.git'
   }
   stage('Build') {
      echo "Run the maven build"
   }
   stage('Notification') {
      echo "Notified to developer"
   }
}