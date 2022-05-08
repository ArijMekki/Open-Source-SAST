# Docker Compose Installation
- The first step is to update the repository, then install the correct version from GitHub:

  `$sudo apt update & sudo apt upgrade & sudo apt install curl`
  
  `$sudo curl -L "https://github.com/docker/compose/releases/download/1.25.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
  
  `$sudo chmod +x /usr/local/bin/docker-compose`

- To verify the correct installation of the tool, we run the command below:

  `$sudo docker–compose –version`
