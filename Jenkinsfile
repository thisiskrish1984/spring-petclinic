node{
    
stage("SCM"){
    //git clone
	git 'https://github.com/thisiskrish1984/spring-petclinic.git'
}
stage("build the package"){
    //mvn package
	sh 'mvn package'
	}
stage("test unit reports"){
	//test unints
	junit 'target/surefire-reports/*.xml'
}	
stage("archival"){
    //archive the artifacts
	archive 'target/*.jar'
	}
}