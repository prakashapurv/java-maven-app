def gv

pipeline {
     agent any
     parameters {
         string(name: 'Version', defaultValue: '', description: 'Version to deploy on Prod')
         choice(name: 'Version', choices: ['1.0','1.1','1.2'], description: '')
     }
     stages {
         stage("init"){
             steps {
                 script {
                     gv = load "script.groovy"

                 }
             }
         }
         stage("build jar") {
             steps {
                 script{
                     echo "Building Jar files"
                 }
             }
         }

         stage("build image"){
             steps{
                 script{
                     echo "Building image from jar"
                 }
             }
         }

         stage ("Deploy Image") {
             steps{
                 script{
	             echo "Deploying the image"

			}
                 }
             }
         }
     }

