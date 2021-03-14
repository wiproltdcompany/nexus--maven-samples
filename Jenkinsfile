pipeline{

      agent {
                docker {
                image 'maven'
                args '-u root -v /home/antara_bits/settings.xml:/root/.m2'
                }
            }
        
        stages{

              stage('deploy'){
                  steps{
                      script{
                            sh "cd demo"
		    	    sh "sudo mvn clean deploy"
		  
                 	}
               	 }  
              }	
		
            }	       	     	         
}
