node ('main'){  
   // def app
    stage('Cloning Git') {
        /* Let's make sure we have the repository cloned to our workspace */
       checkout scm
    }  
    stage('SAST'){
        build 'SECURITY-SAST-SNYK'
    }

    
    stage('Build-and-Tag') {
        sh 'echo Build-andTag'
    /* This builds the actual image; synonymous to
         * docker build on the command line */
    //    app = docker.build("amrit96/snake")
    }
    stage('Post-to-dockerhub') {
    
   /*  docker.withRegistry('https://registry.hub.docker.com', 'training_creds') {
            app.push("latest")
        			}*/
         }     
    stage('Pull-image-server') {
        sh 'echo Pull-image-server'
    
      /*   sh "docker-compose down"
         sh "docker-compose up -d"	
         */
      } 
}
