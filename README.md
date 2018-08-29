# tezos node installation script for betanet



### create new tezos user
$ adduser tezos

$ adduser tezos sudo

$ su - tezos

### install tezos, eneter password for sudo and press Y for all questions
$ sh <(curl -sL https://github.com/atticlab/tezos-node/blob/master/install-tezos.sh)

### after install, check node syncing status
$ cd ./tezos

$ cd ./tezos-client bootstrapped 

### or just check logs 
$ cd ./tazos

$ tail -f nohup.out 



### Updating. Stop the running processes for your node, baker, endorser and accuser.
$ cd ./tezos
$ eval $(opam env)
$ git pull
$ make
