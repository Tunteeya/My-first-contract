# SimpleStorage Smart Contract

## Overview

This project demonstrates the development of a **Solidity** smart contract, implementing fundamental data types, functions, and contract states.
It enables users to store favorite numbers, organize personal data, and manage contract activity through an enum.

This contract was built using the **Remix IDE** and tested locally within the development environment.

## Features

### 1. Data Types and Variables
- **Favorite Number**: A `uint256` variable to store a single favorite number.
- **Array of Favorite Numbers**: A dynamic array (`uint256[]`) to store multiple favorite numbers.
- **Struct for Person**: A `Person` struct to store the name and favorite number of an individual.
- **Enum for Contract State**: A `ContractState` enum to manage contract states (`Active` or `Inactive`).

### 2. Functions
- **storeNumber(uint256 _number)**: Stores the user's favorite number.
- **getFavoriteNumber()**: Returns the stored favorite number.
- **isGreaterThan(uint256 _number)**: Compares the stored favorite number with a given number and returns `true` if it’s greater, otherwise `false`.
- **sumToFavoriteNumber()**: Sums the numbers from `1` to the stored favorite number.
- **addFavoriteNumber(uint256 _number)**: Adds a new favorite number to the dynamic array of favorite numbers.
- **addPerson(string memory _name, uint256 _number)**: Adds a person and their favorite number to the `people` array.
- **activateContract()**: Sets the contract state to `Active`.
- **deactivateContract()**: Sets the contract state to `Inactive`.
- **isActive()**: Checks whether the contract is currently active.

### 3. Visibility Specifiers
- **Private**: The `favoriteNumber` variable is declared as `private`.
- **Public**: The `getFavoriteNumber()` function is publicly accessible.
- **Internal**: An internal function that returns a string, exposed by a public wrapper function.
- **External**: Demonstrates the use of an external function that returns a string and is called using the `this` keyword in a public function.

## How i utilized Remix IDE

1. **Accessing Remix IDE**  
   The process began by visiting [Remix IDE](https://remix.ethereum.org/) in a web browser.

2. **Creating a New Workspace**  
   - The "File Explorers" icon was clicked (the first icon on the left sidebar).
   - A new folder was created by clicking the "+" icon .
3. **Creating a New File**  
   - Inside the newly created folder, a new file named `SimpleStorage.sol` was created by clicking the "+" icon.

4. **Writing the Smart Contract Code**  
   The Solidity code for the smart contract was written directly in `SimpleStorage.sol`, ensuring all necessary features and functions were included.

5. **Compiling the Contract**  
   - The "Solidity Compiler" icon (the second icon on the left sidebar) was clicked.
   - After selecting the appropriate compiler version, the "Compile SimpleStorage.sol" button was clicked.

6. **Deploying the Contract**  
   - The "Deploy & Run Transactions" icon (the third icon) was clicked.
   - The environment was set to "Remix VM (Cancum)" for local testing, followed by deploying the contract by clicking the "Deploy" button.

7. **Pushing to GitHub**  
   After completing the testing, the project was staged and pushed to GitHub. The `README.md` file was later added to document the project and its features.
