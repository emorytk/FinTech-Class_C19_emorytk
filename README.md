OBJECTIVE
This challenge was to build an application for a customer to find a FinTech associate and submit a transaction request>

FILES
The files needed to run this code on Visual Studio are:
* fintech_finder.py
* crypto_wallet.py
* .env
    
IMAGES
The images needed are 
* ash.jpeg
* jo.jpeg
* kendall.jpeg
* lane.jpeg

IMPORTS
The imports needed to run the code for this app are:
* fintech_finder.py
* import streamlit as st
* from dataclasses import dataclass
* from typing import Any, List
* from web3 import Web3
* w3 = Web3(Web3.HTTPProvider('HTTP://127.0.0.1:7545'))

crypto_wallet.py
* import os
* import requests
* from dotenv import load_dotenv
* load_dotenv()
* from bip44 import Wallet
* from web3 import Web3
* from web3 import Account
* from web3 import middleware
* from web3.gas_strategies.time_based import medium_gas_price_strategy


For fintech_finder.py
* Generate a new Ethereum account instance by using your mnemonic seed phrase (which you created earlier in the module).
* Fetch and display the account balance associated with your Ethereum account address.
* Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.
* Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.
* Review the transaction hash code associated with the validated blockchain transaction.
* Once you receive the transaction’s hash code, you will navigate to the Transactions section of Ganache to review the blockchain transaction details. To confirm that you have successfully created the transaction, you will save screenshots to the README.md file of your GitHub repository for this Challenge assignment.

################################################################################

# Imports
* import streamlit as st
* from dataclasses import dataclass
* from typing import Any, List
* from web3 import Web3
* w3 = Web3(Web3.HTTPProvider('HTTP://127.0.0.1:7545'))

################################################################################

Sign and Execute a Payment Transaction
* Fintech Finder customers will select a fintech professional from the application interface’s drop-down menu, input the amount of time for which they’ll hire the worker. The application calculates the amount that the worker will be paid in ether. 

##########################################

Inspect the Transaction
* Send a test transaction by using the application’s web interface, and then look up the resulting transaction hash in Ganache.

* On the resulting webpage, select a candidate that you would like to hire from the appropriate drop-down menu. Enter the number of hours to hire them for. Click the Send Transaction button to sign and send the transaction with your Ethereum account information. If the transaction is successfully communicated to Ganache, validated, and added to a block, a resulting transaction hash code will be written to the Streamlit application sidebar.

Navigate to the Ganache accounts tab and locate your account (index 0). 
* Take a screenshot of the address, balance, and transaction (TX) count. Save this screenshot to the README.md file of your GitHub repository for this Challenge assignment.

Navigate to the Ganache transactions tab and locate the transaction. 
* Click the transaction and take a screenshot of it. Save this screenshot to the README.md file of your GitHub repository for this Challenge assignment.


