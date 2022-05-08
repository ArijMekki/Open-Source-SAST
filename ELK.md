# ELK installation
- you start by installing the github repository below:

  `$git clone https://github.com/deviantony/docker-elk.git`
  
  `$cd /docker-elk`
  
- The first step is to add some changes on the “docker-compose” configuration file to improve the performance of the stack. To install and run the different images you run the command below:

  `$docker-compose up –d`

- After a few second, you can verify that everything is running as expected by executing the command below:

  `$docker ps`
  
  
  > You can access kibana interface by entering http://localhost:5601

