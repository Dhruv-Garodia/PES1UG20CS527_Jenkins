pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
          sh 'g++ ./main/hello.cpp -o ./main/hello'
          echo 'Build successful'
          build job: 'PES1UG20CS527-1'
            }
          }
stage('Test') {
    steps {
		sh './main/hello'
		eho 'Test successful'
			}
}
stage ('Deploy') {
      steps {
        echo 'Deployment Successful'
      }
   }
}
post {
    failure {
echo 'Pipeline failed'
    }
  }
} 
