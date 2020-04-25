pipeline {
	agent any

    stages{
        stage('Init'){
            steps{
                echo "Initialization started ..."
				 sh '''#!/bin/bash
                    npm install
				'''
				echo "....................... "
				echo "Init success..";	
			}
        }

        stage('Unit Test'){
            steps{
               echo "Unit test started ..."
               sh "ng test"
               echo "....................... "
               echo "Unit test success..";	
			}
        }

        stage('Build'){
            steps{
               echo "Build started ..."
				   sh "ng build --prod"
				   echo "....................... "
				   echo "Build success..";	
		   	}
        }
    }
}