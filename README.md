# site

[videoDAC project homepage](http://videodac.eth.link) can be found as part of Livepeer's Protocol Explorer:

This repository explains the setup of videodac.eth.link using ENS and IPFS, to direct a user to [videoDAC project homepage](http://videodac.eth.link).

1. Create `redirect.html`

2. Publish and Pin `redirect.html` to IPFS

Make sure IPFS is running on your localhost.

```
ipfs add redirect.html
```

This will output an IPFS hash, which will look something like this: `QmVFFimGCqqTrkeunZcz65UXXTNHx5hqjGzwzSMkvoCv7p`

```
ipfs pin add QmVFFimGCqqTrkeunZcz65UXXTNHx5hqjGzwzSMkvoCv7p
```

Note: please replace the IPFS hash with the hash generated above.

3. Register the IPFS Hash in ENS

- Go to https://app.ens.domains/

- Click "My Names"

- Create a new "Content" "Record" as below

![image](https://user-images.githubusercontent.com/2212651/82537170-36b52780-9b67-11ea-8d8d-b88fff05c39f.png)

Once the transaction has been mined, the http://videodac.eth.link URL was active
