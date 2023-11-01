pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
  }
  stages {

    stage('Hello') {

      steps {
	sh '''
	git -version
        java -version
        '''
	}
      }
    stage('System Name'){
       steps{
        sh '''

	    whoami
        
        '''
      }
  }
  }
}
