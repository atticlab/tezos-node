# tezos node installation script for betanet



### create new tezos user
$ adduser tezos

$ adduser tezos sudo

$ su - tezos

### install tezos
$sh <(curl -sL https://github.com/atticlab/tezos-node/blob/master/install-tezos.sh)

### after install, check node syncing status
$cd ./tezos

$cd ./tezos-client bootstrapped 

### or just check logs 
$cd ./tazos

$tail -f nohup.out 
