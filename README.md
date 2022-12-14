FundMe:

A Solidity smart contract for managing funding transactions.

Features:
1. Accepts funding transactions in ETH and checks if the amount is above a minimum threshold in USD.
2. Maintains a mapping of addresses to the amount of ETH they have funded.
3. Allows the contract owner to withdraw all funds.

Usage:
1. Deploy the contract, passing the address of an AggregatorV3Interface instance as an argument. This will be used to convert ETH to USD.
2. Call the fund() function to send ETH to the contract. The amount must be at least MINIMUM_USD in USD.
3. Use the withdraw() function to collect all the funds. This can only be called by the contract owner.

License:
This project is licensed under the MIT License
