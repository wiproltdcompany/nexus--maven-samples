pipeline{

      agent {
                docker {
                image 'maven'
                args '-v $HOME/.m2:/root/.m2'
                args '-v /home/antara_bits/settings.xml:/root/.m2'
                }
            }
        
        stages{

              stage('deploy'){
                  steps{
                      script{
                            sh "cd demo"
		    	    sh "mvn clean deploy"
		  
                 	}
               	 }  
              }	
		
            }	       	     	         
}
