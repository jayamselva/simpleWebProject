#!/usr/bin/env groovy

@Library('shared-library@master') _ //master or whatever branch

pipeline{

      agent any
        
        stages{

              stage('maven build'){
                  steps{
                      script{
		    	                sh "mvn package"
                      	  }
               	     }  
                 }	
                 
                 stage ('Check logs') {
                    steps {
                        filterLogs ('WARNING', 1)
                    }
                }
		
           }	       	     	         
}
