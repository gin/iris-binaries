# Note
https://www.irisnet.org/docs/software/How-to-install-irishub.html#compile-source-code

Build testnet binaries after setting env:
`source scripts/setTestEnv.sh`

## testnet
```bash
mkdir -p $GOPATH/src/github.com/irisnet
cd $GOPATH/src/github.com/irisnet
git clone https://github.com/irisnet/irishub
cd irishub && git checkout <latest_iris_version>
make get_tools
source scripts/setTestEnv.sh
make all
```

## mainnet
```bash
mkdir -p $GOPATH/src/github.com/irisnet
cd $GOPATH/src/github.com/irisnet
git clone https://github.com/irisnet/irishub
cd irishub && git checkout <latest_iris_version>
make get_tools
make all
```
