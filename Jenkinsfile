pipeline {
    agent any
    stages {
        stage('Intro') {
                steps {
                        echo 'HTML DOCUMENTATION'
			
                }
        }
	    stage('Ask'){
		    
		steps {
			input('Do you want to proceed?')
        }
	    }
        stage('Resources') {
                steps {
			echo "Hello"
                        }
        }
        stage('Final Stage') {
                parallel {
                        stage('Unit Test') {
                                steps{
                                        echo "Running the unit test..."
                                }
                        }
                        stage('Integration test') {
				steps {
					echo 'Running the integration test..'
				}
                               
			}  }
        }
    }
}
