#Solidity Tutorial
//Other alternative languages to build smart contracts are Rust (limited community and Library support), Vyper(python oriented smart contract), Go, Yul
//Data types: UINT(unsigned Integer), INT(signed Integer), boolean, Enum,etc
//The first thing to do when starting a Smart Contract is to provide a Licence Identifier - SPDX-Licence-Identifier: MIT
//pragma solidity ^0.8.0;

contract dataTypes{
string greeting = "hello";
uint256 num = 9;
} 

contract variableAssignment{
 string public greeting = "hello"; //using the public keyword makes the variable visible (automatically creates a getter function) after deploying the contract
 }

 //we can also assign value to our state variables using the constructor as follows. The constructor keyword runs each time we deploy the contract.

 contract assignValue{
  string public hey;
  uint256 public num;

   constructor(string memory _hey, uint _no){
    hey = _hey;
    num = _no;
   }
   }
