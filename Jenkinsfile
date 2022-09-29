pipeline{
  agent{
    label{
    label "built-in"
    customWorkspace "/mnt"
      
    }
  
  }
  stages{
    stage('installing httpd'){
      steps{
      echo "Installing httpd"
      sh "yum install httpd -y"
      }
    
    }
    
    stages{
    stage('service httpd start'){
      steps{
      echo "httpd start"
      sh "service httpd start"
        sh "checkconfig httpd on"
      }
    
    }
       stages{
    stage('deploy index.html on httpd'){
      steps{
      echo "deploy index.html on httpd"
      sh "sudo cp -r /mnt/index.html /var/www/html"
        sh "sudo chmod -R 777 /var/www/html"
      }
    
    }
  
  }
  
  
}
