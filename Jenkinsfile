node {
     stage('Cont Download from SCM') {
   git 'https://github.com/venkat9822891/maven-project1.git'
                                     }
     stage('Cont Build using maven tool') {
   sh 'mvn package'
                                          }
     stage('cont Deploy into development environment'){										  
  	    deploy adapters: [tomcat9(credentialsId: '31887143-9841-40b0-8c6e-4d512baa9c7f', path: '', url: 'http://172.31.33.184:8080')], contextPath: '/scr-app', war: '**/*.war'                                              
													  }
	 
	 
	 }
