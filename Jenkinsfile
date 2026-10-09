pipeline{
  agent any
  stages{
    stage('''Docker Installation'''){
     steps{
      sh '''
        apt update -y
        apt upgrade -y
        apt install sudo docker.io docker-compose -y
        sudo service docker start
        sudo service docker status
        '''
     }  
    }   
  }
}    
  
