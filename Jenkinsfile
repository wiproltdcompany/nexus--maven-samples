pipeline{

      agent {
                docker {
                image 'maven'
                args '-v /home/antara_bits/settings.xml:/root/.m2'
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
