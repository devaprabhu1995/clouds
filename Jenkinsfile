pipeline {

agent  {
    node {
      label 'node1'
    }
  }
  
      tools {
        jdk 'jdk-8.221'
        maven 'maven-3.8.1'
    }
    
    stages {
        
     stage('Maven version') {
            steps {
                echo "Hello, Maven"
                sh "mvn --version" 
            }
        }
        
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
            
        }
        
        stage('test 1') {
            steps {
                echo 'Stage2 Hello world!'  
                echo  'test 1 $date'
            }
            
        }
        
        
        stage('test 2') {
            steps {
                echo 'Wel come to Stage3 '  
                echo  'test 2 '
            }
            
        }     
      stage('final') {
            steps {
                echo 'the end '  
                echo  'test 3 '
            }
            
        }     
    }
}
