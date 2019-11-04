# BigLittleData

A curated dataset repository with open licenses for machine learning, big data and statistics. It runs under [IPFS](https://ipfs.io/) using Lektor to build the website. The main objectives are:

* Easy interface to download datasets in different formats
* Simple webpage to be able to be used anywhere
* Distributed content using IPFS underlaying.

## Building

Install [Lektor](https://www.getlektor.com/)

```
git clone git@github.com:aarroyoc/biglittledata.git
lektor server (to add/edit/delete datasets)
lektor build -O build
cd build
ipfs add -r .
(get last hash and modify dnslink TXT in DNS provider, pin and keep ipfs alive)
```
HTTPS support thanks to CloudFlare IPFS gateway
