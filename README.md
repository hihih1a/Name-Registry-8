# Name-Registry-8
Name Registry.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract NameRegistry {
    mapping(address => string) public names;

    function setName(string memory _name) public {
        names[msg.sender] = _name;
    }
}
