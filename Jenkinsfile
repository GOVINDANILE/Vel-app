pipeline{
  agent{
    label{
    label "built-in"
    customWorkspace "/mnt"
      
    }
  
  }
  stages{
    staage ('installing httpd'){
      steps{
      echo "Installing httpd"
      sh "yum install httpd -y"
      }
    
    }
  
  }
  
  
}
