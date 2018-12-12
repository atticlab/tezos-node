# tezos node installation script for betanet



### create new tezos user:
$ adduser tezos

$ adduser tezos sudo

$ su - tezos

### install tezos, eneter password for sudo and press Y for all questions:
$ sh <(curl -sL https://raw.githubusercontent.com/atticlab/tezos-node/master/install-tezos.sh)

### after install, check node syncing status:
$ cd ./tezos

$ cd ./tezos-client bootstrapped 

### or just check logs:
$ cd ./tazos

$ tail -f nohup.out 



### updating to new version. stop the running processes for your node, baker, endorser and accuser:
$ cd ./tezos

$ eval $(opam env)

$ git pull

$ make
