

node {
   checkout scm

   def workspace = pwd()
   echo "workspace=${workspace}"
   
   stage 'error'
   def workspace2 = build.getEnvVars()["WORKSPACE"]
        withEnv(["WORKSPACE=${workspace}",
                 "MAKEOBJDIRPREFIX=${makeobjdirprefix}",
                 "BUILD_ROOT=" + pwd(),
                 "MAKE_CONF_FILE=${make_conf_file}",
                 "CONFIG_JSON=" + TEST_CONFIG_FILE ]) {
     echo 'hi'
   }

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
