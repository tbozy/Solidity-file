#Solidity Tutorial
//Other alternative languages to build smart contracts are Rust (limited community and Library support), Vyper(python oriented smart contract), Go, Yul
//Data types: UINT(unsigned Integer), INT(signed Integer), boolean, Enum,etc
//The first thing to do when starting a Smart Contract is to provide a Licence Identifier - SPDX-Licence-Identifier: MIT
//pragma solidity ^0.8.0;

contract dataTypes{
string greeting = "hello"; // first indicate the datatype, then variable name, and then you may or may not assign a value to the variable
uint256 num = 9;  //unsigned integer...only positive integers. uint8 ranges from 1 to 2**8-1//255
bool hey; // default value is false. if we want to make it true then bool public hey = true;
} 

contract variableAssignment{
 string public greeting = "hello"; //using the public keyword makes the variable visible (automatically creates a getter function) after deploying the contract
 }
 //we can also assign value to our state variables using the constructor as follows. The constructor keyword runs each time we deploy the contract.

 contract assignValue{
  string public hey;
  uint256 public num1;

   constructor(string memory _hey, uint _no){
    hey = _hey;
    num1 = _no;
   }
   }
// we can also do this using a function, if we don't need to update the data at the time of deployment

 contract assignValue2{
  string public hey2;
  uint256 public num2;

   function addInfo(string memory _hey, uint _no) public {
    hey2 = _hey;
    num2 = _no;
   }
   }
