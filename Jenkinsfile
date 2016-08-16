

node {
   checkout scm

   def workspace = pwd()
   echo "workspace=${workspace}"
   
   stage 'env'
   echo "BUILD_CAUSE=${env.BUILD_CAUSE}"
   echo "BUILD_ID=${env.BUILD_ID}"
   echo "BUILD_TAG=${env.BUILD_TAG}"
   echo "BUILD_NUMBER=${env.BUILD_NUMBER}"
   echo "BUILD_URL=${env.BUILD_URL}"



/*
   stage 'getRemote'
   def workspace1 = manager.build.workspace.getRemote()
   echo "workspace1=${workspace1}"



   stage 'collect' 
   sh 'git rev-parse HEAD > GIT_COMMIT'
   def shortCommit = readFile('GIT_COMMIT').take(6)
   def image = docker.build("jenkinsciinfra/bind.build-${shortCommit})")

 
   stage 'Deploy'
   image.push()
*/
}
