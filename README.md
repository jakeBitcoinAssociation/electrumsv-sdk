# electrumsv-sdk
BitcoinSV development environment using the Electrumsv-sdk and Docker

## Installation Instructions

1. Make sure you have Docker installed: https://docs.docker.com/get-docker/

  If you're running Apple Silicon, make sure you have rosetta2 installed: (from terminal)

  ```softwareupdate --install-rosetta```

2. clone or download the repo

  ```git clone https://github.com/jakeBitcoinAssociation/electrumsv-sdk.git```

3. cd into the repo directory

4. run docker-compose

  ```docker-compose up -d```

5. Attach to the electrumsv-sdk container to issue commands (see electrumsv-sdk detailed install instructions and github repo for more details)

  ```docker container attach electrumsv-sdk```


The whatsonchain instance is accessible at ```localhost:3002```


Ports for `http://` services (onlocalhost):

    3002      # Whatsonchain
    18332     # Node
    5050      # MAPI
    51001     # ElectrumX
    9999      # ElectrumSV
    49241     # SimpleIndexer
    56565     # StatusMonitor




generate new blocks with ```electrumsv-sdk node generate [num of blocks, e.g. 10]```

To see all available bitcoind RPC commands, run:

```electrumsv-sdk node help```

References

https://electrumsv-sdk.readthedocs.io/en/latest/getting-started/installing-the-SDK.html

https://github.com/electrumsv/electrumsv-sdk

https://github.com/bitcoin-sv/merchantapi-reference/blob/master/README.md
