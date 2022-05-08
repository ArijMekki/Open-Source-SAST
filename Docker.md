# Docker Installation
We begin by updating the Software Repository: </br>
`$sudo apt update` </br>
Then we download used dependencies: </br>
`$sudo apt-get install apt-transport-https ca-certificates curl software-properties-common` </br>
After that, we add Docker’s GPG Key: </br>
`$curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -` </br>
Next, we install the Docker repository: </br>
`$sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs)  stable"` </br>
`$sudo apt update & sudo apt-get install docker-ce` </br>
To ensure that docker is installed correctly we check its version: </br>
` $docker --version` </br>
Then we start and enable the Docker Service: </br>
`$sudo systemctl start docker` </br>
`$sudo systemctl enable docker` </br>
`$sudo systemctl status docker` </br>
To run Docker Commands Without Sudo we add a "docker group" then we associate the username to the created group: </br>
`$sudo groupadd docker` </br>
`$sudo usermod -aG docker sqapp` </br>
` $id -nG` </br>
