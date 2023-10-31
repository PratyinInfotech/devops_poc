pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
  }
  stages {

    stage('Hello') {

      steps {

	step{
	sh '''
	git -version
	'''
	}

	step{

        sh '''

          java -version

        '''
	}
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
