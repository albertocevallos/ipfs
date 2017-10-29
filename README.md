# ipfs_project

## Overview 

This code is a simple JS video player that demonstrates how you can upload simple web https://ipfs.io/ipfs/QmWBygGCzRJ3prhhm9BGP49qPFLzfdVtbSzfxYWForhDNd)apps to IPFS. 

## Dependencies

* IPFS (https://ipfs.io/docs/getting-started/)

## Usage

First, install IPFS using [this](https://ipfs.io/docs/getting-started/) page. 

Then, once you've initalized IPFS and started the daemon see [this](https://ipfs.io/ipfs/QmNZiPk974vDsPmQii3YbrMKfi12KTSNM7XMiYyiea4VYZ/example#/ipfs/QmP8WUPq2braGQ8iZjJ6w9di6mzgoTWyRLayrMRjjDoyGr/websites/README.md) page on how to add this static video player web app to IPFS

## Usecase
DIAC (Digital ID & Authentication Council of Canada) is hosting a design challenge (https://diacc.ca/didc/) and need a blockchain solution for registering land titles in BC.

So far I have succesfully uploaded the image of a land title to IPFS (viewable here: https://ipfs.io/ipfs/QmWBygGCzRJ3prhhm9BGP49qPFLzfdVtbSzfxYWForhDNd)

Once the daemon is running you can add data of any kind (websites, PDFs, Images, Videos) by using the commandline:

`$ ls mysite
img index.html
$ ipfs add mysite -r
added QmcMN2wqoun88SVF5own7D5LUpnHwDA6ALZnVdFXhnYhAs mysite/img/landtitle.jpg
added QmS8tC5NJqajBB5qFhcA1auav14iHMnoMZJWfmr4k3EY6w mysite/img
added QmYh6HbZhHABQXrkQZ4aRRSoSa6bb9vaKoHeumWex6HRsT mysite/index.html
added QmYeAiiK1UfB8MGLRefok1N7vBTyX8hGPuMXZ4Xq1DPyt7 mysite/`

As a result you obtain the last hash and this can be stored in other blockchains (eg. Ethereum) and have a smart contract prove the existence of this document at any point in time. Next, I will create a simple membership website that maps website accounts to Ethereum addresses (ERC20 token compatible) and any land titles under each account.
