

node {
   checkout scm
   
   stage 'env'
   echo "JENKINS_URL=${env.JENKINS_URL}"
   echo "BUILD_URL=${env.BUILD_URL}"

   echo "BUILD_CAUSE=${env.BUILD_CAUSE}"
   echo "BUILD_ID=${env.BUILD_ID}"
   echo "BUILD_NUMBER=${env.BUILD_NUMBER}"
   echo "BUILD_TAG=${env.BUILD_TAG}"

   echo "EXECUTOR_NUMBER=${env.EXECUTOR_NUMBER}"
   echo "HOME=${env.HOME}"
   echo "HUDSON_HOME=${env.HUDSON_HOME}"
   echo "WORKSPACE=${env.WORKSPACE}"
   def workspace = pwd()
   echo "workspace=${workspace}"

   echo "JOB_NAME=${env.JOB_NAME}"
   echo "JAVA_HOME=${env.JAVA_HOME}"

   echo "PWD=${env.PWD}"
   echo "OLDPWD=${env.OLDPWD}"
   echo "JENKINS=${env.JENKINS}"
   echo "USER=${env.USER}"
   echo "TERM=${env.TERM}"

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
