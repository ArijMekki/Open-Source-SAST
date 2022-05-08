# Docker Installation
We begin by updating the Software Repository:
' $sudo apt update '
Then we download used dependencies

> $sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
After that, we add Docker’s GPG Key
> $curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
Next, we install the Docker repository
> $sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs)  stable"
> $sudo apt update & sudo apt-get install docker-ce
To ensure that docker is installed correctly we check its version
> $docker --version
Then we start and enable the Docker Service
> $sudo systemctl start docker
> $sudo systemctl enable docker
> $sudo systemctl status docker
To run Docker Commands Without Sudo we add a "docker group" then we associate the username to the created group:
> $sudo groupadd docker
> $sudo usermod -aG docker sqapp
> $id -nG
