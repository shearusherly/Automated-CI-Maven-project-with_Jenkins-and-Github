pipeline{
    agent any
    stages{
      stage('Start'){
          steps{
          echo 'Start the Pipeline'
          }
      }
        
        
        stage('Clean phase Starts'){
          steps{
          echo 'Start the Clean phase'
          }
      }
      stage('Clean'){
          steps{
          sh 'mvn clean'
          }
      }
        
        stage('Compile phase Starts'){
          steps{
          echo 'Start the Compile phase'
          }
      }
      stage('Compile'){
          steps{
              def mavenHome= tool name: "Maven", type: "maven"
              sh "${mavenHome}/bin/mvn compile"
          //sh 'mvn compile'
          }
      }
      
        
       
        stage('Test phase Starts'){
          steps{
          echo 'Start the Test phase'
          }
      }
        stage('Test'){
          steps{
                 def mvnHome= tool name: "Maven", type: "maven"
       sh "${mvnHome}/bin/mvn test"
          //sh 'mvn test'
          }
      }
       
        
        stage('Install phase Starts'){
          steps{
          echo 'Start the Instll phase'
          }
      }
        stage('Install'){
          steps{
                 def mavenHome2= tool name: "Maven", type: "maven"
       sh "${mavenHome2}/bin/mvn install"
          //sh 'mvn install'
          }
      }
        
        
        
        stage('End'){
          steps{
          echo 'End the pipeline'
          }
      }
    }
}
