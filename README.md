# NITTE INSTITUE OF PROFESSIONAL EDUCATION 
## Team Name :
404: Error
## Problem Statement : 
Fake Product Identification using Blockchain Technology
## Team Members : 
- Abhay R
- Nirmal S Nair
- Pratheeksha
- Nupur Tilakraj Bolar
## Mentor :
Dr. Rakesh S 

## Project Overview
- Our system uses blockchain technology to store and verify product information at each stage of the supply chain. Each product has a unique hash generated based on its details and the hash is stored on the blockchain.
- The system also includes a web application that allows suppliers and buyers to view product information and verify its authenticity.


## Packages Required:-
- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v15.8.0 for the backend
- Web3.js v1.7.4 
- npm 7.5.1
- HTML/CSS for the frontend.

## Other Requirements:-
1. Any chromium based browser i.e. Chrome 
2. Metamask browser extension
3. Anaconda Prompt
    
## Setup process 

1. Clone the project
```
git clone https://github.com/abhayr10/Fake_Product_Detection.git
```
2. Open anaconda prompt, go to the approppriate project folder using 'cd' command to change directories, and run following command to install required node_modules:-
```
npm install
```
3. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-
```
truffle compile
```

4. Open Ganache, (to setup local blockchain)
    - Create new workspace
    - Add truffle-config.js  in truffle project 
    - Change port to 7545 in server settings (same as port in truffle-config.js)
5. In chrome, open metamask 
   - Add new test network using  
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:8545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - Import account using private key of any account from local blockchain available in Ganache.
6. In terminal, run following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```

- Run the command below to start a server and it will open a homepage (index.html) file in the default browser.
```
npm run dev 
``` 
7. Login to metamask ,and connect the added account to local blockchain (i.e.localhost:3000)
8. Interact with the website opened 
