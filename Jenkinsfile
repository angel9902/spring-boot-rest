// comment
pipeline {
 agent any
 environment { 
        PATH '/opt/maven3/bind:$PATH' 
    }
 stages {
	 stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }	 
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
			sh 'mvn --version'
		}
	}
  }
}

