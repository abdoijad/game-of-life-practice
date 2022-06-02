pipeline {

      agent {
	  
	  node {
	        
			label "built-in"
			customWorkspace "/mnt/project"
			}
			}

    stages {


        stage ("Install Stage") {
            steps {
		                    
                    sh "mvn install"
		    
		   
                }
            
        }
	    stage ("Docker-Compose-Deploy"){
	       
	        steps {
	           
	            sh "docker-compose up -d --scale webserver=3"
				
				
    }
}
    }
}

