# README

## Overview

This code demonstrates the implementation of a Singleton design pattern for managing bank branch information. The Singleton pattern ensures that only one instance of a class is created and provides a global point of access to that instance.

## Implementation

1. **Singleton Instance Variable**
   - A variable named `bankBranchInstance` is created to store the singleton instance of the bank branch.

2. **BankBranch Class**
   - A class called `BankBranch` is defined for managing branch information.

3. **Constructor**
   - The constructor of the `BankBranch` class takes `branchInfo` as a parameter.
   - Inside the constructor, it checks if the `bankBranchInstance` variable is null (indicating no instance exists).
     - If `bankBranchInstance` is null, it creates a new instance with the provided `branchInfo` and assigns it to `bankBranchInstance`.
     - If `bankBranchInstance` is not null, it returns the existing `bankBranchInstance`.

4. **Methods**
   - Methods are added to the `BankBranch` class for managing branch-related information.
   - The `getBranchInfo` method retrieves branch information.

## Usage

- Instances of the `BankBranch` class, such as `branchA` and `branchB`, are created with different branch information.
- The `getBranchInfo` method is used to retrieve branch information from the instances.
- It's verified that `branchA` and `branchB` are both referring to the same instance by comparing them using `===`.

## Dependencies

- JavaScript