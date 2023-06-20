# Assignment Contract

## Overview
This repository contains the smart contract code for the Assignment contract. The contract demonstrates the usage of `require()`, `assert()`, and `revert()` statements to handle conditions and ensure the desired behavior of the contract.

The contract includes functionalities related to a solar panel machine, a weather changer, and bringing an umbrella. It allows users to check if it is sunny, generate solar power, change the weather condition, and determine the need for an umbrella based on the current weather.

## Contract Details

- **Solidity Version**: 0.8.18
- **License**: MIT

## Functionalities

### Solar Panel Machine
The `solar` function is used to generate solar power. It uses the `require()` statement to check if it is sunny. If the condition fails, the function execution is reverted. Otherwise, it adds 3 to the `finalCal` variable. The `assert()` statement is used to verify that `finalCal` is not equal to 6.

### Weather Changer
The `weatherChanger` function allows users to change the weather condition. It toggles the `sunny` variable between `true` and `false`.

### Bringing Umbrella
The `BringUmbrella` function determines if an umbrella needs to be brought. If it is not sunny, the `umbrella` variable is set to `true`. Otherwise, the function execution is reverted with an error message using the `revert()` statement.

### Get Final Cal
The `getCal` function is a view function that returns the value of the `finalCal` variable.

## Deployment and Usage

To deploy the contract, follow these steps:

1. Compile the smart contract code using a Solidity compiler (e.g., Remix, Truffle).
2. Deploy the contract to an Ethereum network of your choice (e.g., local development network, public testnet, or mainnet) using a compatible Ethereum client or development framework (e.g., Remix, Truffle, Hardhat).

Once deployed, you can interact with the contract using the provided functions:

- Use the `solar` function to generate solar power, which adds 3 to `finalCal`. Make sure it is sunny, or the transaction will be reverted.
- Use the `weatherChanger` function to toggle the weather condition between sunny and not sunny.
- Use the `BringUmbrella` function to determine if an umbrella needs to be brought based on the weather. If it is not sunny, the `umbrella` variable will be set to `true`. Otherwise, the transaction will be reverted.
- Use the `getCal` function to retrieve the value of the `finalCal` variable.

## Development Environment

The contract is developed using Solidity version 0.8.18. It is recommended to use a compatible Solidity compiler or development framework (e.g., Remix, Truffle) for compilation and deployment.

## License

This project is licensed under the [MIT License](LICENSE).
