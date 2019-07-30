// Powered by Infostretch 

timestamps {

node () {

	stage ('jfrog job - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '7dd389b9-8403-43db-9028-6cdaf32db70a', url: 'https://github.com/Jyothinayak123/Jyothi.git']]]) 
	}
	stage ('jfrog job - Build') {
 	
// Unable to convert a build step referring to "org.jfrog.hudson.generic.ArtifactoryGenericConfigurator". Please verify and convert manually if required.		// Shell build step
sh """ 
mvn compile package 
 """ 
	}
}
}