The [Rupee Blockchain](https://rupeeblockchain.org/) wallet for Ubuntu _(version 1.0.0)_ currently only works on `Ubuntu 14.04`. This is due to the fact that a package that the wallet uses (`libboost-thread1.58.0`) is only available in the Ubuntu 14.04 repositories.
Because most Ubuntu computers are now 16.04 or 18.04, getting this wallet to work can be hard. The following commands should help you get the wallet up and and running for later systems.
```
# sudo apt-cache search libboost-system  
# sudo apt-get install libminiupnpc-dev  
# sudo vim /etc/apt/sources.list  
...  
deb http://gr.archive.ubuntu.com/ubuntu xenial main  
...  
# sudo apt-cache search libboost-system  
# sudo apt-get install libboost-system-dev libboost-system1.58.0 # libboost-filesystem1.58.0 libboost-program-options1.58.0 libboost-thread1.58.0  
# sudo apt-get install libqt5printsupport5  
# sudo apt install libqrencode3  
# sudo apt-get install software-properties-common  
# sudo add-apt-repository ppa:bitcoin/bitcoin  
# sudo apt-get update  
# sudo apt-get install -y libdb4.8-dev libdb4.8++-dev
```
