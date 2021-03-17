# Install global dependencies
- you will need Node, we are using version 14.4
```
npm install -g truffle ganache-cli
```

# Metamask setup
- follow this https://docs.matic.network/docs/develop/metamask/config-matic/


# Install package dependencies
- in the root folder
  ```
  nvm use
  yarn install
  ```

# Generate Mnemonic
- create a file in the root folder: `touch .secret`
- Generate a new 12-word mnemonic using https://iancoleman.io/bip39/
- paste the mnemonic into the `.secret` file
  
# Compile
`truffle compile`

# Local Deployment

  ## Deploy on Ganache 
  - ganache is a local ethereum network
  - start ganache in a separate terminal: `ganache-cli`
  - deploy the smart contract, in a separate terminal:
  ```
  truffle migrate --network development
  ```

  OR 

  ## Deploy on Truffle Local blockchain
  (https://www.trufflesuite.com/docs/truffle/getting-started/using-truffle-develop-and-the-console)
  ```
  truffle develop
  ```


# Deploying on Matic Network
Run this command in root of the project directory:
```
$ truffle migrate --network matic
```
