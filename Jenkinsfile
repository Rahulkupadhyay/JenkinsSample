pipeline {
	agent any

    stages{
        stage('Init'){
            steps{
               script {
                  sh '''
                  #!/bin/bash -xe
                  echo "Initialization started ..."
                  sh "npm install"
                  echo "....................... "
                  echo "Init success..";	
                  '''
               }
			}
        }

        stage('Unit Test'){
            steps{
               script {
                  sh '''
                  #!/bin/bash -xe
                  echo "Unit test started ..."
                  sh "ng test"
                  echo "....................... "
                  echo "Unit test success..";	
                  '''
               }
			   }
        }

        stage('Build'){
            steps{
               script {
                  sh '''
                  #!/bin/bash -xe
                  echo "Build started ..."
                  sh "ng build --prod"
                  echo "....................... "
                  echo "Build success..";	
                  '''
               }
		   	}
        }
    }
}