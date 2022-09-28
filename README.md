# python-for-devops-october-2022
From Zero Repository for doing Python DevOps work


![Drawing sketchpad](https://user-images.githubusercontent.com/60753177/192761015-5838aab5-fd95-4b3a-bc75-bc8f146478b8.png)


## Create a project scaffold

  * Create development environment that is cloud-based : 
  
    ### Colab Notebook :
    
    This is an example of how to use [colab] (https://github.com/Leon-dipac/python-for-devops-october-2022/blob/main/getting_started_with_python.ipynb)
    
    ### GitHub Codespaces : This is a paid service under the GitHub Account.
    
    Build out python project scaffold :
    
    * Create a ' Makefile '
    * create a ' requirements.txt '
    * Create a ' test_library.py '
    * python_library
    * Dockerfile
    * command-line-tools
    * Microservices


    ### AWS CloudShell : It's an alternative cloud environment to GitHub Codespaces
    
    ### AWS Cloud9 : It's an alternative cloud environment to GitHub Codespaces. You can just set up your Cloud9 environment 
    with a 't2.micro' with Amazon Linux AMI.
    
    Name of the environment : " python-devops-october-2022 "
    Description of the environment : " This is for coding with Python. "
    
    Once your Cloud9 environment is created then run the following command :
      -> Clone your repository using the 'SSH' Link :
      $ git clone git@github.com:Leon-dipac/python-for-devops-october-2022.git
      
      NB: When you create a new environment, you will have 'Permission denied (publickey)' error when cloning a GitHub Repo.
      
      -> Generate a once off key by typing the command then press 'enter' 3 times : 
      
      $ ssh-keygen -t rsa
      
      -> Your generated public key will be saved in your EC2 instance :
      
      $ cat {public key EC2 instance location }
      
       For example : 
       
      $ cat /home/ec2-user/.ssh/id_rsa.pub
      
      Please follow the video at 42 minutes to get the GitHub steps :
        Link : https://www.youtube.com/watch?v=kwZNpieUreA
        
      -> create a python virtual environment : 
      $ python3 -m venv ~/.venv
      $ vim ~/.bashrc
      
      In the insert mode add the following at the bottom :
      
      # Sourcing the virtual environment
      source ~/.venv/bin/activate
      
      then press " :wq "
      
      -> Now open a new terminal and type the following commands to verify that no legacy library has been installed in your new environment :
      
      $ which python
      $ pip freeze | wc -l




## Command -Lines Tools

## Microservices

## Containerized Continuous Delivery

