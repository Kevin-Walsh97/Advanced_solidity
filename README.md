# Advanced_solidity

# Deploying Contracts

## Deploying PupperCoinSaleDeployer.sol

To begin, we will deploy the PupperCoinSaleDeployer contract, as this will set up all the pieces of the other contract. Before we deploy, we first need to connect to the Kovan network. 

[Kovan_network](Images/Kovan_network.png)

Once we have done that, we can proceed with deploying our PupperCoinSaleDeployer contract and initializing the parameters like so. For the address for our wallet, we can copy and past the information from the "ACCOUNT" field above. 

[Deployed_puppercoindeployer](Images/Deployed_puppercoindeployer.png)

Once we have successfully deployed the contract, we will see three "buttons". The first is an orange one denoting the fastforward functionality that we built into the contact. The second two are address objects: token_address and token_sale_address. We will need to leverage this to continue the deployment of our other crowd sale contracts.

[success_1](Images/success_1.png)

## Deploying PupperCoinSale

After deploying this contract, we can deploy the PupperCoinSale at the token_sale_address object, which we have conveniently found in the previous step.  

[At_sale_address](Images/At_sale_address.png)

This will cause another deployed contract to populate below with the functionality that we previously built in. 

[success_2](Images/success_2.png)

## Deploying PupperCoin

The next step is deploying the PupperCoin contract. This time, we will be deploying at the token_address that we had previously found.

[At_token_address](Images/At_token_address.png)

This will cause a third deployed contract to populate below with the functionality that we previously built in. 

[success_3](Images/success_3.png)

# Buying Tokens

Once we have successfully deployed the contracts above we can then proceed with transacting our tokens. By grabbing another one of our test ether wallets in Ganache, we can buy tokens by converting our test ETH to tokens. 

[Buy_1](Images/Buy_1.png)

We can confirm that this transaction went through by using the "balanceOf" object to see how many tokens are now populated in that account. 

[Balance_of](Images/balanceOf.png)



