// comment
pipeline {
 agent any
 stages {
        stage('Git-Clone'){
               steps{
		  echo "Se obtiene el código fuente del proyecto de Spring-Boot-Rest"
		  	git poll: false,
				url : 'https://github.com/angel9902/spring-boot-rest.git'
		  echo "Se obtiene el código fuente de manera correcta"
               }
        }
	stage('Maven'){
		steps{
		   echo "Se ejecuta maven"
			sh 'maven clean compile'
		}
	}
  }
}

