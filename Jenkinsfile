pipeline {
    agent any
	
    stages {
        stage('Build') {
		
			when{
				changelog "build====to stage"
			}
		
            steps {                
                echo 'Hello World changing request'
                echo "hello"
            }
        }
        stage("Deploy stage"){
            when{
                changelog "Deployed"
            }
               steps {                
                echo 'deployed to staging'
            }
        }
    }
}