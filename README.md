Wildfire Multi Tool script tested on Linux 18.04
(Automatic IPv6 configuration is valid only for U18 contabo servers)

Wildfire MN install guide




Commands to install wildfiremultitool.sh

wget https://github.com/Wildfire-new/Wildfire-multitool/blob/master/wildfiremultitool.sh

chmod +x wildfiremultitool.sh

./wildfiremultitool.sh


New server note
New server and IPv6 setup only needs to be set up once per server.


MultiNode note
To run multiple MN's on one server you will need to use the IPv6 option when promted in option 6 enter a unique Alias, BLS secret key, and rpc port each time you run masternode install tool.


Masternode install note

Alias = Name of your MN, Must all be in lower case with no spaces or special characters and also include "scc" in the name for multi tools

secret key= get this from your control wallets console using the command

bls generate

note this info and enter carefully

Port = Default port is 40000 and is set for you

RPCport = Default RPCport is 39999 use unique for multinode


Check.sh instructions (This will be replaced with the health check and repair tool soon)

Updated check.sh file for new commands if you are using an older version of this script
wget 

chmod +x check.sh

The new server option will also add a file in root named check.sh
edit this file using 
nano check.sh
add node alias to "node="
example "node1=alias"
