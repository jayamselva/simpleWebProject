#!/usr/bin/env groovy

@Library('shared-library@master') _ //master or whatever branch

pipeline{

      agent any
        
        stages{

              stage('maven build'){
                  steps{
                      script{
		    	                echo "Hello Selva"
                      	  }
               	     }  
                 }	
                 
                 stage ('Check logs') {
                    steps {
                        filterLogs ('Hello', 1)
                    }
                }
		
           }	       	     	         
}
