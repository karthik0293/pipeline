pipeline {
	agent any  
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') { 
			parallel {
				stage('TEST1') {
					steps {
						sh 'sleep 5'
					}
				}
				stage('TEST2') {
					steps {
						sh 'sleep 5'
					}
				}
			}
		}
				

		
		stage('DEPLOY') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: DEPLOY
				'''
			}	
		}
	}
}
