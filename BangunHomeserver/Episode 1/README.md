## YouTube Video

YouTube Link: [Episode 1](https://youtu.be/mNEXuJcmz7c)

## Install Docker

```text
sudo apt-get update
```
```text
sudo apt-get install ca-certificates curl gnupg lsb-release
```
```text
sudo mkdir -p /etc/apt/keyrings
```
```text
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
```
```text
echo \
"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```text
sudo apt-get update
```
```text
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```
```text
sudo service docker start
```
```text
sudo docker run hello-world
```
## Install Portainer
```text
docker run -d -p 9000:9000 --restart always --name portainer -v /opt/portainer-data:/data -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer
```
