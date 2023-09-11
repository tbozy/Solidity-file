#Solidity Tutorial
//Other alternative languages to build smart contracts are Rust (limited community and Library support), Vyper(python oriented smart contract), Go, Yul
//Data types: UINT(unsigned Integer), INT(signed Integer), boolean, Enum,etc
//The first thing to do when starting a Smart Contract is to provide a Licence Identifier - SPDX-Licence-Identifier: MIT
//pragma solidity ^0.8.0;

contract variableTypes{
string greeting = "hello";
uint256 num = 9;
} 

contract variableAssignment{
 string public greeting = "hello"; //using the public keyword makes the variable visible after deploying the contract
 }
 //we can also assign value to our state variables using the constructor as follows:

 contract assignValue{
  string public hey;
  uint256 public num;
  
