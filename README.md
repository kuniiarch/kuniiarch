sudo apt update && sudo apt upgrade -y
sudo apt install nodejs && sudo apt install git
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" 
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y
sudo apt install npm
sqd init your username -t https://github.com/subsquid-quests/single-chain-squid
npm install --global @subsquid/cli@latest
cd your username
sqd up
npm ci
sqd build
sqd migration:apply
sqd run
