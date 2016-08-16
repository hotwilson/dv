

node {
   checkout scm

   def workspace = pwd()
   echo "workspace=${workspace}"
   
   stage 'error'
   def version = "${env.BUILD_ID}"
   // def myVar = build.getEnvironment(listener).get('BUILD_ID')

   stage 'getRemote'
   def workspace1 = manager.build.workspace.getRemote()
   echo "workspace1=${workspace1}"


/*
   stage 'collect' 
   sh 'git rev-parse HEAD > GIT_COMMIT'
   def shortCommit = readFile('GIT_COMMIT').take(6)
   def image = docker.build("jenkinsciinfra/bind.build-${shortCommit})")

 
   stage 'Deploy'
   image.push()
*/
}
