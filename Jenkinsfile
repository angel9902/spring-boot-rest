pipeline {
 agent any
 
 tools {
    maven 'M3'
  }
  
 stages {
        stage('Git-Clone'){
               steps{
		  echo "Se obtiene el código fuente del proyecto de Spring-Boot-Rest"
		  	git poll: false,
				url : 'https://github.com/angel9902/spring-boot-rest.git'
		  echo "Se obtiene el código fuente de manera correcta"
               }
        }
    	stage('Maven-Compile'){
    		steps{
    		   echo "Se inicia la compilación del código fuente"
    			 sh 'mvn clean compile'
    		   echo "Se compila correctamente el código fuente"	
    		}
    	}
    /*	stage('Maven-Deploy'){
    		steps{
    		    echo "Se inicia el deploy del código fuente"
    		        sh 'mvn clean deploy'
    	    }
    	}
    */
        
    
  }
}
