node {
	stage ('SCM checkout'){
		git "https://github.com/saigieeshchinthakani/selenium-Jenkinspipeline.git"
		}
	stage ('Build'){
    	dir("comtest") {
	   bat "mvn clean install"
       }
	}
    stage ('test') {
    	bat "java -jar comtest/target/com.test-1.0-SNAPSHOT.jar"
    }
}

