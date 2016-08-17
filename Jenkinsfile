#!/usr/bin/env groovy

/**
 * Sample Jenkinsfile for Jenkins2 Pipeline
 * from https://github.com/hotwilson/jenkins2/edit/master/Jenkinsfile
 * by Wilson Mar@gmail.com 
 */
 
import hudson.model.*
import hudson.EnvVars
import groovy.json.JsonSlurperClassic
import groovy.json.JsonBuilder
import groovy.json.JsonOutput
import java.net.URL

node {
//   checkout scm
   
   stage '\u2776 env'
   /* Only keep the 10 most recent builds. */
properties([[$class: 'BuildDiscarderProperty',
                strategy: [$class: 'LogRotator', numToKeepStr: '10']]])

   echo "BUILD_CAUSE=${env.BUILD_CAUSE}"
   echo "BUILD_ID=${env.BUILD_ID}"
   echo "BUILD_NUMBER=${env.BUILD_NUMBER}"
   echo "BUILD_TAG=${env.BUILD_TAG}"
   echo "JENKINS_URL=${env.JENKINS_URL}"
   echo "\u2600 BUILD_URL=${env.BUILD_URL}"

   echo "EXECUTOR_NUMBER=${env.EXECUTOR_NUMBER}"
   echo "HOME=${env.HOME}"
   echo "HUDSON_HOME=${env.HUDSON_HOME}"
   echo "WORKSPACE=${env.WORKSPACE}"
   def workspace = pwd()
   echo "\u2600 workspace=${workspace}"

   echo "JOB_NAME=${env.JOB_NAME}"
   echo "JAVA_HOME=${env.JAVA_HOME}"

   echo "PWD=${env.PWD}"
   echo "OLDPWD=${env.OLDPWD}"
   echo "JENKINS=${env.JENKINS}"
   echo "USER=${env.USER}"
   echo "TERM=${env.TERM}"

   echo "LANG=${env.LANG}"
   echo "LOGNAME=${env.LOGNAME}"
   echo "NODE_NAME =${env.NODE_NAME}"
   echo "GIT_COMMIT  =${env.GIT_COMMIT}"
   echo "GIT_URL =${env.GIT_URL}"
   echo "GIT_BRANCH =${env.GIT_BRANCH}"
   echo "CVS_BRANCH  =${env.CVS_BRANCH}"
   echo "SVN_REVISION =${env.SVN_REVISION}"

   stage '\u2777 remote'

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
