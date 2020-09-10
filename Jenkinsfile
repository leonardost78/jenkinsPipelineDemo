node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      echo 'Running pipeline from Jenkingfile'
      echo 'Checking out the code'
      git 'https://github.com/leonardost78/jenkinsPipelineDemo.git'
      sh 'ls'
      sh 'chmod 755 *.sh'
   }
   stage('Build') {
      // Run the maven build
      sh './build.sh'
   }
   stage('Package') {
      // Run the maven build
      sh './package.sh'
   }
   stage('Test') {
      // Run the maven build
      sh './test.sh'
   }
   stage('Deploy') {
      // Run the maven build
      sh './deploy.sh'
   }   
}
