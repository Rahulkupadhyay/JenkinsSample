pipeline {
	agent any

    stages{
        stage('Init'){
            steps{
               echo "Initialization started ..."
               bat label: '', script: ' npm install'
               echo "....................... "
               echo "Init success..";	
			}
        }

        stage('Unit Test'){
            steps{
               echo "Unit test started ..."
               echo "....................... "
               echo "Unit test success..";	
			}
        }

        stage('Build'){
            steps{
               echo "Build started ..."
               bat label: '', script: ' ng build --prod'
				   echo "....................... "
				   echo "Build success..";	
		   	}
        }
    }
}