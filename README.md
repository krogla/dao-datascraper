# DAO-datascraper
[![Build Status](https://travis-ci.org/PeterChauYEG/dao-datascraper.svg?branch=master)](https://travis-ci.org/PeterChauYEG/dao-datascraper)

A node app that pull transaction data about the DAO (0xbb9bc244d798123fde783fcc1c72d3bb8c189413) from Etherscan.io and exports it as a .csv or .json file.

Donations: 0x1A416af553Faca53b4be48DCFB6E749C9737455D

[Powered by Etherscan.io APIs][Powered by Etherscan.io APIs]

## [Latest Release][Latest Release]

## How to use

1. Clone this repo with ```git clone https://github.com/PeterChauYEG/dao-datascraper.git``` or with [Cloud9 IDE][Cloud9 IDE]
2. [Install Node][install node]
3. Install NPM packages with: ```npm install```
4. Update the settings.js file with the account address and other options
5a. Get the entire DAO transaction log as a CSV: ```npm start```
5b. Get the entire DAO transaction log as a json: ```npm start -- json``` or ```npm run-script export-json```
6. Your .csv or .json file can be found in the ```output/``` folder in the format ```YYYY-MM-DD```

Note: the etherscan api returns a maximum of 10000 transaction (tx) records for this query. If your total number of tx is more than 10k you may want to adjust the startblock number in settings.js and run this multiple times to get the full list of tx.

[Cloud9 IDE]: https://c9.io/c/JVUChbVycba
[Latest Release]: https://github.com/PeterChauYEG/dao-datascraper/releases/tag/v1.0.5
[install node]: https://nodejs.org/en/
[Powered by Etherscan.io APIs]: https://etherscan.io/apis
[Home Page]: http://peterchauyeg.github.io/dao-datascraper/
