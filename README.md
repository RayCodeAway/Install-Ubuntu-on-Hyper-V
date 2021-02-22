# Install Ubuntu WSL For Cosmos


# run remote desktop
sudo /etc/init.d/xrdp start

# shutdown WSL
wsl --shutdown

# to download
wget -c https://golang.org/dl/go1.16.linux-amd64.tar.gz
# to checksum file
shasum -a 256 go1.7.3.linux-amd64.tar.gz

# extract zipped file
sudo tar -C /usr/local -xvzf go1.16.linux-amd64.tar.gz

# setting evironment path
export PATH=$PATH:/usr/local/go/bin

# Save a File in Vim / Vi #
The command to save a file in Vim is :w.

To save the file without exiting the editor, switch back to normal mode by pressing Esc, type :w and hit Enter.

# goto folder and created subfolder
 cd /home/akhtar/ && mkdir Downloads

# remove folder
sudo mv /home/xxxxxxx/tendermint/build/tendermint /usr/local/bin/

# cosmos tendermint build

# Environment variables only run once
echo export GOPATH=\"\$HOME/go\" >> ~/.bash_profile

echo export PATH=\"\$PATH:\$GOPATH/bin\" >> ~/.bash_profile

# SET Environment variables in windows
source ~/.bash_profile
source ~/.profile

after running command below.. move the binary to shared/root folder

make install

# Once youve build the project.. the binary must be moved to a generic folder

sudo mv /home/akhtar/tendermint/build/tendermint /usr/local/bin/

# run the tendermint binary
rm -rf ~/.tendermint

tendermint init

tendermint node --proxy-app=kvstore

# Check Netstats to see SPID blocking port
sudo netstat -ltnp | grep ':26656'

"tcp6       0      0 :::26656                :::*                    LISTEN      14099/tendermint   "

Kill 14099

# run starport
curl https://get.starport.network/starport@v0.13.1 | bash

# move starpot binary to local/root
sudo mv /home/akhtar/starport /usr/local/bin/

# vscode in WSL 
setup github
  git config --global user.email "akhtar.miah@hotmail.com"
  git config --global user.name "coderayway"
