#!groovy

node {
	   
	stage('Checkouting'){

          //checkout scm
git branch: 'stage', credentialsId: '5d9f9895-2946-4a9d-a5f6-6a516623d1fe', url: 'https://github.com/gmanoj23/Maven-Web-Project.git'

       }

       stage('BuildArtifact'){

          sh 'mvn install'
       }
	   
      stage('Sonar') {
                    //add stage sonar
                    sh 'mvn sonar:sonar'
                }
       
}
