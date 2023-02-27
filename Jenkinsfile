pipeline {
	agent any
	parameters {
  string defaultValue: 'QA', description: '''QA
UAT
DEV''', name: 'env'
}

	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/pallavi/Documents/GRASS/apache-maven-3.9.0/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/Stringpara.war /home/pallavi/Documents/GRASS/apache-tomcat-9.0.72/webapps'
	}
}}}
