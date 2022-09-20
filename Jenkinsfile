pipeline {
	agent any
        triggers {
        	pollSCM('*/10 * * * *')
	}
	stages {
		stage("Compile") {
			steps {
				sh "./gradlew compileJava"
			}
		}
		stage("Unit test") {
			steps {
				sh "./gradlew test"
			}
		}
	}
} 
