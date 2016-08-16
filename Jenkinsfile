

node {
   checkout scm
   def workspace = "hello"
   echo "workspace=${workspace}"
   
   stage 'getRemote'
   def workspace = manager.build.workspace.getRemote()
   
   stage 'error'
   def workspace = manager.build.getEnvVars()["WORKSPACE"]


/*
   stage 'collect' 
   sh 'git rev-parse HEAD > GIT_COMMIT'
   def shortCommit = readFile('GIT_COMMIT').take(6)
   def image = docker.build("jenkinsciinfra/bind.build-${shortCommit})")

 
   stage 'Deploy'
   image.push()
*/
}
