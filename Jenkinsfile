pipeline {
	agent any
	stages{
		   stage ('Build') {
				steps {
					echo "Build step..."
					sh 'mvn clean package'
				}
				post {
				    success {
				        echo 'Archiving'
				    }
				}
		   }
		   stage ('Deploy') {
				steps {
					echo "Deploy step..."
				}
		   }
	}
}
