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
				println "Init success..";	
			}
        }

        stage('Unit Test'){
            steps{
                echo "Unit test started ..."
				 sh '''#!/bin/bash
                    ng test
				'''
				echo "....................... "
				println "Unit test success..";	
			}
        }

        stage('Build'){
            steps{
                echo "Build started ..."
				 sh '''#!/bin/bash
                    ng build --prod
				'''
				echo "....................... "
				println "Build success..";	
			}
        }
    }
}