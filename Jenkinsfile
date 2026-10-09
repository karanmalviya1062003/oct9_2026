pipeline{
  agent any
  parameters{
    string(name: 'FOOD_NAME', defaultValue: 'tomato')
    string(name: 'VEGETABLE', defaultValue: 'potato')
  }
  stages{
    stage('''Docker Installation'''){
     steps{
      sh '''
        apt update -y
        apt upgrade -y
        apt install vim sudo -y
        vim --version
        apt install sudo docker.io docker-compose -y
        sudo service docker start
        sudo service docker status
        '''
        sudo docker image pull ubuntu:latest
        sudo docker images
     }  
    }   
  }
}    
  
